---
api_specs:
- filename: tesseract-public-api-openapi.json
  format: json
  label: Tesseract Public API
  slug: tesseract-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesseract/refs/heads/main/openapi/tesseract-public-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tesseract.fi
  spf: true
hosts:
- cert_expires: Aug 31 10:03:54 2026 GMT
  host: tesseract.fi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 15:26:35 2026 GMT
  host: docs.tesseract.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: api.vault.tesseract.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tesseract Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tesseract, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tesseract
provider_slug: tesseract
slug: tesseract-domain-security
source_filename: tesseract-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tesseract.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:03:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.tesseract.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:26:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vault.tesseract.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tesseract.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesseract/refs/heads/main/security/tesseract-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Cryptocurrency
- DeFi
- Lending
- Yield
- Digital Assets
- Ethereum
- MiCA
- Vaults
- Institutional
---
