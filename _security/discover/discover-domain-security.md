---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: discoverglobalnetwork.com
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: partner.discoverglobalnetwork.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Discover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Discover, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Discover
provider_slug: discover
slug: discover-domain-security
source_filename: discover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partner.discoverglobalnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: discoverglobalnetwork.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discover/refs/heads/main/security/discover-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Credit Cards
- Fortune 500
---
