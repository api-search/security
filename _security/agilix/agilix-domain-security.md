---
description: ''
domains:
- caa:
  - 0 issuewild "cloudflare.com"
  - 0 iodef "mailto:it@agilix.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "cloudflare.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agilix.com
  spf: true
- caa:
  - 0 issuewild "cloudflare.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "cloudflare.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agilixbuzz.com
  spf: true
hosts:
- cert_expires: Nov 27 05:51:28 2026 GMT
  host: www.agilix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 19:02:07 2026 GMT
  host: api.agilixbuzz.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: backgroundapi.agilixbuzz.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agilix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agilix, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agilix
provider_slug: agilix
slug: agilix-domain-security
source_filename: agilix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agilix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 05:51:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.agilixbuzz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 19:02:07 2026 GMT\n  hsts: null\n- host: backgroundapi.agilixbuzz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: agilix.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"cloudflare.com\"\n  - 0 iodef \"mailto:it@agilix.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: agilixbuzz.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"\
  cloudflare.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agilix/refs/heads/main/security/agilix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Learning Management System
- K-12
- Online Learning
- Tutoring
- Assessment
- LTI
- SCORM
- Artificial Intelligence
- Event
---
