---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: helipaddy.com
  spf: true
hosts:
- cert_expires: Aug 19 07:01:52 2026 GMT
  host: helipaddy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helipaddy Sites Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helipaddy sites, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Helipaddy sites
provider_slug: helipaddy-sites
slug: helipaddy-sites-domain-security
source_filename: helipaddy-sites-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helipaddy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:01:52 2026 GMT\n  hsts: false\ndomains:\n- domain: helipaddy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helipaddy-sites/refs/heads/main/security/helipaddy-sites-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vehicle
- Public APIs
---
