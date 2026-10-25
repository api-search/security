---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:dnsadmins@syneoshealth.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: syneoshealth.com
  spf: true
hosts:
- cert_expires: Dec 26 07:36:59 2026 GMT
  host: www.syneoshealth.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- host: developer.syneoshealth.com
  https: false
- cert_expires: Dec 28 12:56:41 2026 GMT
  host: api.syneoshealth.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Syneos Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syneos Health, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Syneos Health
provider_slug: syneos-health
slug: syneos-health-domain-security
source_filename: syneos-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.syneoshealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 07:36:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.syneoshealth.com\n  https: false\n- host: api.syneoshealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 12:56:41 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: syneoshealth.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:dnsadmins@syneoshealth.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syneos-health/refs/heads/main/security/syneos-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Clinical Research
- Biopharmaceutical
- Contract Research Organization
- Life Sciences
- Healthcare
- Commercialization
---
