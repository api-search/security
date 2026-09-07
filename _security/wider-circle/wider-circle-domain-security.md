---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@widercircle.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: widercircle.com
  spf: true
hosts:
- cert_expires: Nov 11 04:24:43 2026 GMT
  host: www.widercircle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 00:44:46 2026 GMT
  host: portal.widercircle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Wider Circle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wider Circle, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wider Circle
provider_slug: wider-circle
slug: wider-circle-domain-security
source_filename: wider-circle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.widercircle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 04:24:43 2026 GMT\n  hsts: false\n- host: portal.widercircle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 00:44:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: widercircle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@widercircle.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wider-circle/refs/heads/main/security/wider-circle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Plans
- Medicare Advantage
- Medicaid
- Population Health
- Social Determinants of Health
- Member Engagement
- Care Coordination
- Community Health
---
