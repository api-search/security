---
api_specs:
- filename: tmt-id-verify.yml
  format: yaml
  label: TMT Verify API
  slug: tmt-id-verify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-verify.yml
- filename: tmt-id-velocity.yml
  format: yaml
  label: TMT Velocity API
  slug: tmt-id-velocity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-velocity.yml
- filename: tmt-id-live.yml
  format: yaml
  label: TMT Live API
  slug: tmt-id-live
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-live.yml
- filename: tmt-id-teleshield.yml
  format: yaml
  label: TMT TeleShield API
  slug: tmt-id-teleshield
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-teleshield.yml
- filename: tmt-id-score.yml
  format: yaml
  label: TMT Score API
  slug: tmt-id-score
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-score.yml
- filename: tmt-id-authenticate.yml
  format: yaml
  label: TMT Authenticate API
  slug: tmt-id-authenticate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-authenticate.yml
- filename: tmt-id-network-biometrics.yml
  format: yaml
  label: Network Biometrics API
  slug: tmt-id-network-biometrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-network-biometrics.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tmtid.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tmtanalysis.com
  spf: true
hosts:
- cert_expires: Oct 19 21:46:21 2026 GMT
  host: tmtid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 13:56:12 2026 GMT
  host: viteza.tmtanalysis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.tmtverify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tmt Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TMT ID, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TMT ID
provider_slug: tmt-id
slug: tmt-id-domain-security
source_filename: tmt-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tmtid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 21:46:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: viteza.tmtanalysis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 13:56:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tmtverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tmtid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tmtanalysis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/security/tmt-id-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Telecommunications
- United Kingdom
- Identity Verification
- Mobile Identity
- SIM Swap
- Anti-Fraud
- Number Intelligence
- Silent Network Authentication
- GSMA Open Gateway
- Network APIs
- ENUM
- KYC
---
