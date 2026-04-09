# Cache
- Utilizamos cache para processos que demandam muito tempo, como por exemplo uma busca no banco de dados, que batem em várias tabelas.
- E se uma das tabelas quase nunca mudar? Nesse caso faz ainda mais sentido
## Problema
- Difícil de lidar em larga escala pois possíveis informações as vezes ficam erradas, visto que os dados da aplicação podem mudar (exemplo: Imagem do Github, que demora um tempo para atualizar).
- Exemplos de bancos para cache: MemCached, DragonFly, Redis
- IMPORTANTE: Deve ser implementado na camada de Infra.