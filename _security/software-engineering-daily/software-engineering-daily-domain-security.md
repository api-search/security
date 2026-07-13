---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: softwareengineeringdaily.com
  spf: true
hosts:
- cert_expires: Aug 18 05:24:02 2026 GMT
  host: softwareengineeringdaily.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Software Engineering Daily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software Engineering Daily, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Software Engineering Daily
provider_slug: software-engineering-daily
slug: software-engineering-daily-domain-security
source_filename: software-engineering-daily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: softwareengineeringdaily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:24:02 2026 GMT\n  hsts: false\ndomains:\n- domain: softwareengineeringdaily.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software-engineering-daily/refs/heads/main/security/software-engineering-daily-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Media
- Podcasts
- Software Engineering
- Technical Content
- Open Source
---
