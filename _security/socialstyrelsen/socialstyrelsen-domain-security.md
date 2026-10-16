---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: socialstyrelsen.se
  spf: true
hosts:
- cert_expires: Jan 23 14:08:10 2027 GMT
  host: www.socialstyrelsen.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Socialstyrelsen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Socialstyrelsen (National Board of Health and Welfare), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Socialstyrelsen (National Board of Health and Welfare)
provider_slug: socialstyrelsen
slug: socialstyrelsen-domain-security
source_filename: socialstyrelsen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.socialstyrelsen.se\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 14:08:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: socialstyrelsen.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socialstyrelsen/refs/heads/main/security/socialstyrelsen-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Government
- Health
- Sweden
- PublicPolicy
- Healthcare
---
