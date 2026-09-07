---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 011h.com
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: 011h.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 02:51:53 2026 GMT
  host: api.011h.com
  hsts: false
  https: true
  note: Resolves to an AWS-hosted Kong API gateway that answers every probed path with {"message":"no Route matched with those values"} (HTTP 404). No public routes, docs or spec are exposed anonymously.
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 011H Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 011h, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 011h
provider_slug: 011h
slug: 011h-domain-security
source_filename: 011h-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts; api.011h.com added from STEP 0b contract discovery\n  (DNS resolves, Kong gateway)\nhosts:\n- host: 011h.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: false\n- host: api.011h.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 02:51:53 2026 GMT\n  hsts: false\n  note: Resolves to an AWS-hosted Kong API gateway that answers every probed path with {\"message\":\"no Route matched\n    with those values\"} (HTTP 404). No public routes, docs or spec are exposed anonymously.\ndomains:\n- domain: 011h.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/011h/refs/heads/main/security/011h-domain-security.yml
summary_line: TLSv1.3
tags:
- Construction
- Construction Technology
- Real Estate
- Proptech
- Sustainability
- Building
- Manufacturing
- Spain
- Company
---
