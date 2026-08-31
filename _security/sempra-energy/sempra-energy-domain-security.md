---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sempra-energy.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sempra.com
  spf: true
hosts:
- cert_expires: Oct 28 04:49:43 2026 GMT
  host: www.sempra-energy.com
  hsts: false
  hsts_source: HEAD https://www.sempra-energy.com/ -> 301 to https://www.sempra.com/ with no Strict-Transport-Security header
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: developer.sempra.com
  hsts: true
  hsts_max_age: 63072000
  hsts_preload: true
  hsts_source: 'GET https://developer.sempra.com/ -> 200, Strict-Transport-Security: max-age=63072000; preload'
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.sempra.com
  hsts: true
  hsts_max_age: 86400
  hsts_source: 'GET https://api.sempra.com/ -> 404, Strict-Transport-Security: max-age=86400'
  https: true
  tls_version: TLSv1.2
- host: www.sempra.com
  hsts: false
  https: true
  note: 'Cloudflare managed challenge (cf-mitigated: challenge); GET / returns 403 with no Strict-Transport-Security header.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sempra Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sempra Energy, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sempra Energy
provider_slug: sempra-energy
slug: sempra-energy-domain-security
source_filename: sempra-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts; HSTS values corrected by hand-probe (see\n  hsts_note)\nhosts:\n- host: www.sempra-energy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 04:49:43 2026 GMT\n  hsts: false\n  hsts_source: HEAD https://www.sempra-energy.com/ -> 301 to https://www.sempra.com/ with no Strict-Transport-Security\n    header\n- host: developer.sempra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_preload: true\n  hsts_source: 'GET https://developer.sempra.com/ -> 200, Strict-Transport-Security: max-age=63072000;\n    preload'\n- host: api.sempra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n  hsts_source: 'GET https://api.sempra.com/ -> 404, Strict-Transport-Security: max-age=86400'\n- host: www.sempra.com\n  https: true\n\
  \  tls_version: TLSv1.3\n  hsts: false\n  note: 'Cloudflare managed challenge (cf-mitigated: challenge); GET / returns 403 with no Strict-Transport-Security\n    header.'\ndomains:\n- domain: sempra-energy.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: sempra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nhsts_note: probe-domain-security.py reads HSTS from a HEAD request and treats any non-2xx as \"unknown\".\n  api.sempra.com answers HEAD / with an Apigee 404 and developer.sempra.com answers HEAD / with 403 for\n  the probe user-agent, so both were recorded as null on the automated pass. A hand GET on 2026-08-28\n  shows BOTH hosts do serve Strict-Transport-Security; the values below are the observed ones. www.sempra.com\n  sits behind a Cloudflare managed challenge (403) and served no HSTS header on the challenge response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sempra-energy/refs/heads/main/security/sempra-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Energy
- Utilities
- Natural Gas
- Electricity
- Energy Infrastructure
- LNG
- Apigee
---
