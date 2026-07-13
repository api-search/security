---
api_specs:
- filename: defillama-openapi.yml
  format: yaml
  label: DefiLlama Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defillama/refs/heads/main/openapi/defillama-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: defillama.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: llama.fi
  spf: false
hosts:
- cert_expires: Aug 20 06:27:35 2026 GMT
  host: defillama.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 20:27:49 2026 GMT
  host: api.llama.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 13:55:53 2026 GMT
  host: pro-api.llama.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defillama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DefiLlama, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: DefiLlama
provider_slug: defillama
slug: defillama-domain-security
source_filename: defillama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: defillama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:27:35 2026 GMT\n  hsts: false\n- host: api.llama.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:27:49 2026 GMT\n  hsts: null\n- host: pro-api.llama.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 13:55:53 2026 GMT\n  hsts: null\ndomains:\n- domain: defillama.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: llama.fi\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defillama/refs/heads/main/security/defillama-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Web3
- DeFi
- TVL
- Crypto
- Stablecoins
- Yields
- Bridges
- Aggregator
- Open Source
---
