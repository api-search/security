---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: incrediblehq.com
  spf: true
hosts:
- cert_expires: Dec 12 01:23:15 2026 GMT
  host: incrediblehq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Incrediblehq Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Incredible Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Incredible Health
provider_slug: incrediblehq-com
slug: incrediblehq-com-domain-security
source_filename: incrediblehq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incrediblehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 01:23:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: incrediblehq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/incrediblehq-com/security/incrediblehq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- TalentMarketplace
- AI
- Staffing
---
