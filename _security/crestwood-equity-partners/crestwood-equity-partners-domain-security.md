---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crestwoodlp.com
  spf: true
hosts:
- host: www.crestwoodlp.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Crestwood Equity Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crestwood Equity Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crestwood Equity Partners
provider_slug: crestwood-equity-partners
slug: crestwood-equity-partners-domain-security
source_filename: crestwood-equity-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crestwoodlp.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: crestwoodlp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crestwood-equity-partners/refs/heads/main/security/crestwood-equity-partners-domain-security.yml
summary_line: DMARC
tags:
- Acquired
- Crude Oil
- Energy
- Energy Transfer
- Gathering
- Midstream
- Natural Gas
- NGL
- Pipelines
- Processing
- Storage
- Transportation
---
