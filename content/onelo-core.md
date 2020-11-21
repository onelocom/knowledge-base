+++
id = "onelo-core"
+++

# Onelo Core

Onelo Core is a transformation pipeline starting with a set of files and ending with another set of files.

We can split this pipeline in a different phases:

* __Prelude__: Set up contextual information such as the version of Onelo.
* __Sourcing__: Gather all relevant information given a source.
* __Extraction__: Parse all source entries, extract and generate structures.
* __Transformation__: Apply tranformation rules to generate the desired output.

![Pipeline diagram](https://kroki.io/bpmn/svg/eNq9WltzmzgUfs-vYNiX3ZlujDAYnKnTaZO0szNNm0m6ffVgkG1ibuHi269fgSSMMJKVBO9Laox0zvd950g6Ou7HT9swUNYwzfw4mqjgUlMVGLmx50eLifrvr69_2-qn64uPsySMrjw49yM_RyMzBU2Lsqvy64m6zPPkajDYbDaXcbi4jNPFIEugO_jycP9joGtA00zdGNz_vL37rjYmer7s1Nt_6DzP5c-5vW3MuKln-JIzah8zPz54KYFe-vEgc5cwdKrHQTkgDuJ0UMnlexP19qDMVNv75hKsVCV30gXMfzghzBLHhSKTSPRtEqc5TCfqjRMWkeco97EHA5geXv2mUTIudeT4-kJRcFySNHZhllVIHvDnqWZkhu_sEbzsbgvdIndmAYKQpwWsZtK5GUKZ361hlFfTn-rHKSDj6Mi4yBcxSovrr0G8mWoQrPeL7OOAfYctD1qmmw5zJ1tVrj67ub_2891UCw0z3I1UJUJSIf5L6K6UGwep00Lgo8QMawSgcF5saBNn9TsRZvcF7IJQhLlE10QLt25QZP4afnNyuHF2FXLyeQpcuHD1tRAl61MGJVg9G46x60TJmRGkxjzXRbzaPJgUgC8FWvOwtFXxawJXlSwuUhc-wnlXyHCOVy_bqiiDE2GHi_XGc2jYH6HjKU-VL3HYGXmkBN3Z61Hgvibs3ZIQ1xQxyu8AMvocSdCQ55j3KX22-nyfGtTbl8IPqEAyq4MhLSVTun6ehXYPMmHXnMyh7DuloZQHEl5w0kvrX7_zktH-JWn5QAIJ1jmZItSbWYPderdmMHpLRchPNE1LRRFq85DQEcPgRIsGRFrIjjyOx8Z-3bXOZdKYoSwl0sjPk2TeQxpj190JRrl3ZjElfFKY4TjYWOwC_5Y6yVIsCUNQSpLn1Wb3bPUgCXbNyRVKu1sTwvWEJiDRxxsjo5p8TpJgpzwWAczEmjAMpTTR_U1uRT1ogl3zNCG0uzSpuZ7SZDxOV15ONflZ5EmRi-VgyMmVRvMXYz7rQQ7suluOmnGnHJQmIweMvEN1igtTzd748yg5UXY1-bAK0JKIWJYphSpjHE4UdoMTi_NkfAPNXYU6je8TzIsT5JjaWyrbmVr5HeElrhkpmDtDd2gpQ5lzHUPliE0Nde4xtChlvCzSuEjwcV5-mmrBdoHub6rior18Eae7305QYDc3zW-mmgXTfbI-YQ54S8tYr0-bA0aQbJP0FLos2lmFJ2EOmP58NzyFLhiBYKtJkJ3lhr4HxBxJCXKvPFw0qZXKAzWA5u6cOGGvlYw_ZnhL3HX5iFbMNk8dt7xAK8nSySALhFo7hQStRZB54auQ1HEhSKrSBC2O9-DQguTZsPLX4aABJTh-pU6UzeM0dN6riqaPdyMwf118aD4QNA8pDAoPSsHw_KuyfXPrO4vUCSvjjee6r9Ac-xA4EaxHVk_lXlKOuAtgiLaW484Gs98RO3feAh5tJVPPb5liNhpqB1lCVlB1l6C9MVe2E3VooZWzm6jAOhQuXeNMu2sclqcB7DRgsrtyANO9lw9EB7YUYN3qCzA-GXmAybnJBwLssZzEYDzS-4FMChReUpDyRYDE0iUhW-OeVCYlJg8yKUAFSExTEvJI7wsyvinwIJN7hADJ0JaEbJh9Qcb3PR5kchsUINGBKQdZ72u_IHd3HmRysxcgARpGopepKoIMxq8dqOnv5IYbKjxupPvDR2LZktEAI7OnaOC-Fw8x6YrxkYwNSY21zqi9BTFuaPIQk3anQONRV7AF404ws3kKNBh8d2YwOLwqjbhXX-Ii8jLsaohN6Ojfje_lS_TZUJUl9BfLvNwvWMsDnuk3nYZVy5x7GuKGOp_-SHLPs4ZvztinpZNgxNP6cdq4wOkt5J2_B7U1BzY5m81xrflwdNB8OOLBrPyLcbavd8fqHl8Ayx_oruZ-EEzUP-az-cybcbHXtdvQqrFXuyIFb2vvAN9qSB9jP-pY-9m9k65g-tvP_PYvdh3ZTjPB1Gv0ZgO8qfWiPO7Zi5QnXX0eznphl4B6V7ndrhYBpQ3tRoqki9mfuml-UHTd-KAAy_6Ln-n11nsWInU2WKPk2RwL0qX1i8QRzvpQO29i4JavSG_SFOYC1c-6_tqNWCFS0qptZ4amocwYln80IMiMug49LxHSQhUQqZusLSLAtsoU19EfU0SkvgOcmQjum4qIkM4qF2l9wToLUqaJewyzuxd9hLG-t571bCR9UZGYtHP6irOxbhOc52xstmM7tjqmW8vfP0hp2diPh6ABcai9uZREtA1s-0C_rHTeV0pKK0M6yzxlaOOZp4xxLIxl9SOMrVltXcpK9H_ShbTIuRlDOuj8_U07EgYYPWXMaDg8UqZx-dCt82YM7vZzM4b8GCBQpi1MdTr3IIxOypGmLqDHjGG-r9rHhwY1246-viBt68Z_Zry--A9jrYq8)

_Update previous diagram using [this bpmn file](assets/pipeline.bpmn) and [kroki.io](https://kroki.io)._

## Phases

TODO: Add some description of each phase

### Prelude

### Sourcing

### Extraction

### Transformation

## Cache

The content get from the files in the __sourcing__ phase is persisted in a cache to facilitate its subsequent management.

### Cache data model

![Cache data model diagram](https://kroki.io/erd/svg/eNqdUUtrxCAQvs-vkO0tIZC9FNq_EsriYxKkrgYzWRpK_3tX85Y0h950vudoJZ0l_KIP9i0a6Yzz7-zyUotaKHH5gewTB3hw0yNA1bneS0yZQry-BaZW4F1PCKTv2BG_t4vkhpb8cCLMJ144ck9Yc0nhEstZutHQRhCqGT0xm0RPsnUqqatKLFU5EUmTQVDYSa9b0s5CbrRF3oxF0vBdM6iesEUZZH9FOK8bbQM7I-4bjMKD0NVpzfpXkcg4WdhwgWbnHdWL-cmjwvYnWVYUVzZO9sC1KHI21zuAtmkA4X_CPGPrDstwDhjlyzjxWMdLKqxmBz4bMG6RvF4iTtL2YLZk_gJ7GCF0)

_Update previous diagram using [this erd file](assets/cache-data-model.erd) and [kroki.io](https://kroki.io)._

TODO: Add small description of each table

* source
* source_entry
* content_type
* artefact
* node
* connection
* connection_type
* context

## Onelo Core API

TODO: Use this features to improve this documentation

* Read a directory recursively (all subdirectories included) and get the filename of all files inside
* Read a file and get all the contents
* Store file content in the cache
* Get file content from cache
* Get all files from cache according to its location in the filesystem
* Get a graph according to the relationships between them:
  * Links in their content
  * Connections created in their metadata
  * Inferred by its content
* Create and write files according content stored in the cache