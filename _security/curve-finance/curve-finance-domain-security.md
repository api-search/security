---
api_specs:
- filename: curve-finance-crvusd-api-openapi.yml
  format: yaml
  label: Curve Finance crvUSD API
  slug: curve-finance-crvusd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curve-finance/refs/heads/main/openapi/curve-finance-crvusd-api-openapi.yml
- filename: curve-finance-deprecated-api-openapi.yml
  format: yaml
  label: Curve Finance Deprecated API
  slug: curve-finance-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curve-finance/refs/heads/main/openapi/curve-finance-deprecated-api-openapi.yml
- filename: curve-finance-gauges-api-openapi.yml
  format: yaml
  label: Curve Finance Gauges API
  slug: curve-finance-gauges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curve-finance/refs/heads/main/openapi/curve-finance-gauges-api-openapi.yml
- filename: curve-finance-lending-api-openapi.yml
  format: yaml
  label: Curve Finance Lending API
  slug: curve-finance-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curve-finance/refs/heads/main/openapi/curve-finance-lending-api-openapi.yml
- filename: curve-finance-misc-api-openapi.yml
  format: yaml
  label: Curve Finance Misc API
  slug: curve-finance-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curve-finance/refs/heads/main/openapi/curve-finance-misc-api-openapi.yml
- filename: curve-finance-pools-api-openapi.yml
  format: yaml
  label: Curve Finance Pools API
  slug: curve-finance-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curve-finance/refs/heads/main/openapi/curve-finance-pools-api-openapi.yml
- filename: curve-finance-tokens-api-openapi.yml
  format: yaml
  label: Curve Finance Tokens API
  slug: curve-finance-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curve-finance/refs/heads/main/openapi/curve-finance-tokens-api-openapi.yml
- filename: curve-finance-volumes-and-apys-api-openapi.yml
  format: yaml
  label: Curve Finance Volumes and APYs API
  slug: curve-finance-volumes-and-apys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curve-finance/refs/heads/main/openapi/curve-finance-volumes-and-apys-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@worldethicaldata.org"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: curve.fi
  spf: true
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@worldethicaldata.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: curve.finance
  spf: true
hosts:
- cert_expires: Aug 22 04:38:54 2026 GMT
  host: curve.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 15:48:24 2026 GMT
  host: docs.curve.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 15:48:24 2026 GMT
  host: api.curve.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curve Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curve Finance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Curve Finance
provider_slug: curve-finance
slug: curve-finance-domain-security
source_filename: curve-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curve.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 04:38:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.curve.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:48:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.curve.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:48:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curve.fi\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@worldethicaldata.org\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: curve.finance\n  dnssec: true\n  caa:\n  - 0 issuewild\
  \ \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@worldethicaldata.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curve-finance/refs/heads/main/security/curve-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- DeFi
- DEX
- AMM
- Stablecoins
- Pegged Assets
- Multi-Chain
- Open-Source
---
