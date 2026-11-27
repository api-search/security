---
anonymous_access: false
api_key_in: []
api_specs:
- filename: packagento-com-openapi-generated.yml
  format: yaml
  label: Packagento API
  slug: packagento-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packagento-com/openapi/_ae-authored/packagento-com-openapi-generated.yml
auth_types: []
description: Authentication for Packagento packages is performed using HTTP Basic credentials derived from a project token (public_key/private_key pair).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Packagento Authentication
name_suffix: Authentication
oauth_flows: []
overview: Packagento declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Packagento
provider_slug: packagento-com
scheme_count: 1
schemes:
- evidence: Composer uses them as HTTP Basic credentials when it fetches metadata or downloads a package.
  header: Authorization
  how_to_obtain: Sign in to Packagento, go to Projects & Tokens, create a token for the desired project, and copy the public_key (username) and private_key (password) into auth.json.
  location: header
  name: Packagento Composer token
  type: http-basic
slug: packagento-com-authentication
source_filename: packagento-com-authentication.yml
source_heading: Authentication Profile
source_url: https://packagento.com/mageplaza/module-two-factor-authentication.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://packagento.com/mageplaza/module-two-factor-authentication.md\nsources:\n- https://packagento.com/mageplaza/module-two-factor-authentication.md\n- https://packagento.com/docs/api-tokens\n- https://packagento.com/docs/composer-setup\n- https://packagento.com/docs/vendor-onboarding\ndescription: Authentication for Packagento packages is performed using HTTP Basic credentials derived from a project token (public_key/private_key\n  pair).\nschemes:\n- type: http-basic\n  name: Packagento Composer token\n  evidence: Composer uses them as HTTP Basic credentials when it fetches metadata or downloads a package.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in to Packagento, go to Projects & Tokens, create a token for the desired project, and copy the public_key (username) and\n    private_key (password) into auth.json.\ndocs: https://packagento.com/mageplaza/module-two-factor-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/packagento-com/authentication/packagento-com-authentication.yml
summary_line: 1 scheme
tags:
- Marketplace
- Magento
- Composer
- PHP
- E-Commerce
---
