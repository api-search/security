---
api_specs:
- filename: buymeacoffee-webhooks-openapi.json
  format: json
  label: Buy Me a Coffee Webhooks
  slug: buymeacoffee-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buymeacoffee/openapi/buymeacoffee-webhooks-openapi.json
- filename: buymeacoffee.postman_collection.json
  format: json
  label: Buy Me a Coffee Extras API
  slug: buymeacoffee-extras-api
  spec_type: Postman
  url: https://artifacts.apis.io/buymeacoffee/collections/buymeacoffee.postman_collection.json
- filename: buymeacoffee.postman_collection.json
  format: json
  label: Buy Me a Coffee Subscriptions API
  slug: buymeacoffee-subscriptions-api
  spec_type: Postman
  url: https://artifacts.apis.io/buymeacoffee/collections/buymeacoffee.postman_collection.json
- filename: buymeacoffee.postman_collection.json
  format: json
  label: Buy Me a Coffee Supporters API
  slug: buymeacoffee-supporters-api
  spec_type: Postman
  url: https://artifacts.apis.io/buymeacoffee/collections/buymeacoffee.postman_collection.json
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: buymeacoffee.com
  spf: true
hosts:
- cert_expires: Jan  2 21:45:16 2027 GMT
  host: www.buymeacoffee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 21:45:16 2027 GMT
  host: help.buymeacoffee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 21:45:16 2027 GMT
  host: developers.buymeacoffee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Buy Me a Coffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buy Me a Coffee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Buy Me a Coffee
provider_slug: buymeacoffee
slug: buymeacoffee-domain-security
source_filename: buymeacoffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buymeacoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:45:16 2027 GMT\n  hsts: false\n- host: help.buymeacoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:45:16 2027 GMT\n  hsts: false\n- host: developers.buymeacoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:45:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buymeacoffee.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/buymeacoffee/security/buymeacoffee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Creator Economy
- Membership
- Subscription
- Tips
- Payments
- Donations
---
