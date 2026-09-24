---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: merlinnetwork.org
  spf: true
hosts:
- cert_expires: Dec 18 16:06:32 2026 GMT
  host: merlinnetwork.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Merlin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merlin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Merlin
provider_slug: merlin
slug: merlin-domain-security
source_filename: merlin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merlinnetwork.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 16:06:32 2026 GMT\n  hsts: false\ndomains:\n- domain: merlinnetwork.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merlin/refs/heads/main/security/merlin-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Music
- Licensing
- Technology
- Membership
---
