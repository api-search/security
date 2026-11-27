---
api_specs:
- filename: sukuk-fi-openapi-generated.yml
  format: yaml
  label: SukukFi API
  slug: sukuk-fi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sukuk-fi/openapi/_ae-authored/sukuk-fi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: sukuk.fi
  spf: true
hosts:
- cert_expires: Jan 26 10:37:27 2027 GMT
  host: sukuk.fi
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SukukFi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SukukFi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SukukFi
provider_slug: sukuk-fi
slug: sukuk-fi-domain-security
source_filename: sukuk-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sukuk.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 10:37:27 2027 GMT\n  hsts: false\ndomains:\n- domain: sukuk.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/sukuk-fi/security/sukuk-fi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Blockchain
- IslamicFinance
- Telecom
- CreditMarketplace
---
