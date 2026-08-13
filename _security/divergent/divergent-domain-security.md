---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: divergent.us
  spf: true
hosts:
- cert_expires: Sep 14 18:52:51 2026 GMT
  host: www.divergent.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Divergent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Divergent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Divergent
provider_slug: divergent
slug: divergent-domain-security
source_filename: divergent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.divergent.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:52:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: divergent.us\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nx-legacy-domain:\n  domain: divergent3d.com\n  note: >-\n    Divergent's former primary domain. The apex 301s to https://www.divergent.us/ but\n    presents an EXPIRED TLS certificate, so any strict client aborts the handshake before\n    it ever sees the redirect. www.divergent3d.com does not complete a TLS handshake at\n    all (connection times out). Every inbound link, press release and search result still\n    pointing at divergent3d.com is therefore broken for conforming clients. Recorded\n    2026-08-12; observed with curl, which reported \"\
  SSL certificate problem: certificate\n    has expired\".\n  apex_tls: expired\n  apex_redirect_target: https://www.divergent.us/\n  www_reachable: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/divergent/refs/heads/main/security/divergent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Manufacturing
- Additive Manufacturing
- 3D Printing
- Industrial
- Aerospace
- Defense
- Automotive
- Robotics
- Generative Design
---
