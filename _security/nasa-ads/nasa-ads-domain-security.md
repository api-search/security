---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: harvard.edu
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: ui.adsabs.harvard.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nasa Ads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NASA ADS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: NASA ADS
provider_slug: nasa-ads
slug: nasa-ads-domain-security
source_filename: nasa-ads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ui.adsabs.harvard.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: harvard.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-ads/refs/heads/main/security/nasa-ads-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Science And Math
- Public APIs
---
