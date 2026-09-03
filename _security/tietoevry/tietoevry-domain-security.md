---
api_specs:
- filename: tietoevry-openbanking-xs2a-swagger.json
  format: json
  label: Tietoevry Open Banking XS2A APIs
  slug: tietoevry-openbanking-xs2a
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tietoevry/refs/heads/main/openapi/tietoevry-openbanking-xs2a-swagger.json
- filename: tietoevry-financial-api-aggregation-swagger.json
  format: json
  label: Tietoevry Financial API Aggregation
  slug: tietoevry-financial-api-aggregation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tietoevry/refs/heads/main/openapi/tietoevry-financial-api-aggregation-swagger.json
- filename: tietoevry-sepa-direct-debit-api-gateway.yaml
  format: yaml
  label: Tietoevry SEPA Direct Debits
  slug: tietoevry-sepa-direct-debits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tietoevry/refs/heads/main/openapi/tietoevry-sepa-direct-debit-api-gateway.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tietoevry.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "dvv.fi"
  - 0 issuewild "fineid.fi"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tieto.com
  spf: true
hosts:
- cert_expires: Nov 15 14:44:37 2026 GMT
  host: www.tietoevry.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: openbanking.api.tietoevry.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: aggregation.api.tieto.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tietoevry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TietoEVRY, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TietoEVRY
provider_slug: tietoevry
slug: tietoevry-domain-security
source_filename: tietoevry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tietoevry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 14:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: openbanking.api.tietoevry.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\n- host: aggregation.api.tieto.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tietoevry.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tieto.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"dvv.fi\"\n  - 0 issuewild \"fineid.fi\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tietoevry/refs/heads/main/security/tietoevry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Open Banking
- PSD2
- XS2A
- Berlin Group
- Payments
- SEPA
- Account Information
- Financial Services
- Aggregation
- Credit
- Fintech
- Nordic
- Finland
---
