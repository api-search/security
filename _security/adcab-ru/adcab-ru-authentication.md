---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Yandex Direct API via OAuth2
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AdCab Authentication
name_suffix: Authentication
oauth_flows: []
overview: AdCab declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AdCab
provider_slug: adcab-ru
scheme_count: 1
schemes:
- evidence: 'Токен передаётся в каждом запросе заголовком Authorization: Bearer ТОКЕН .'
  flows:
  - authorizationCode
  - implicit
  how_to_obtain: Create an OAuth application at https://oauth.yandex.ru/client/new to obtain ClientID and Client secret.
  name: Yandex OAuth
  type: oauth2
slug: adcab-ru-authentication
source_filename: adcab-ru-authentication.yml
source_heading: Authentication Profile
source_url: https://adcab.ru/blog/api-yandeks-direkta-kak-poluchit-dostup-i-token-poshagovo
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://adcab.ru/blog/api-yandeks-direkta-kak-poluchit-dostup-i-token-poshagovo\nsources:\n- https://adcab.ru/blog/api-yandeks-direkta-kak-poluchit-dostup-i-token-poshagovo\ndescription: Authentication for Yandex Direct API via OAuth2\nschemes:\n- type: oauth2\n  name: Yandex OAuth\n  evidence: 'Токен передаётся в каждом запросе заголовком Authorization: Bearer ТОКЕН .'\n  flows:\n  - authorizationCode\n  - implicit\n  how_to_obtain: Create an OAuth application at https://oauth.yandex.ru/client/new to obtain ClientID and Client secret.\ndocs: https://adcab.ru/blog/api-yandeks-direkta-kak-poluchit-dostup-i-token-poshagovo\n"
source_yaml_url: https://artifacts.apis.io/adcab-ru/authentication/adcab-ru-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- Artificial Intelligence
- Marketing
- Russian
- Integration
---
