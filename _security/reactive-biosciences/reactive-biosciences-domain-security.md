---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1;p=reject;sp=reject;pct=100;ri=86400;fo=1;
  dnssec: false
  domain: reactivebio.com
  mx: reactivebio-com.mail.protection.outlook.com
  note: Email is on Microsoft 365; strong outbound email posture (SPF hard-fail plus DMARC p=reject). No CAA and no DNSSEC.
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
- caa: []
  dmarc: false
  dnssec: false
  domain: reactivebiosciences.com
  note: Parked/for-sale lander (GoDaddy parking); returns HTTP 200 for every path including /.well-known/* and /security.txt, so those responses are not genuine endpoints. No API or developer surface.
  spf: false
hosts:
- cert_cn: '*.wpengine.com'
  cert_expires: Mar  2 23:59:59 2027 GMT
  cert_matches_host: false
  host: reactivebio.com
  hsts: false
  https: true
  note: TLS terminates on WP Engine with a wildcard *.wpengine.com certificate that does not match the host; the site returns HTTP 404 "not configured", i.e. the public website is not yet launched.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reactive Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reactive Biosciences, probed live across 1 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reactive Biosciences
provider_slug: reactive-biosciences
slug: reactive-biosciences-domain-security
source_filename: reactive-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the organization domain (apis.yml declares no\n  API hosts; company website is pre-launch, so the registrable org domain was probed\n  directly)\nhosts:\n- host: reactivebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  cert_cn: '*.wpengine.com'\n  cert_matches_host: false\n  hsts: false\n  note: TLS terminates on WP Engine with a wildcard *.wpengine.com certificate that\n    does not match the host; the site returns HTTP 404 \"not configured\", i.e. the\n    public website is not yet launched.\ndomains:\n- domain: reactivebio.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: v=DMARC1;p=reject;sp=reject;pct=100;ri=86400;fo=1;\n  mx: reactivebio-com.mail.protection.outlook.com\n  note: Email is on Microsoft 365; strong outbound email posture (SPF\
  \ hard-fail plus\n    DMARC p=reject). No CAA and no DNSSEC.\n- domain: reactivebiosciences.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: Parked/for-sale lander (GoDaddy parking); returns HTTP 200 for every path\n    including /.well-known/* and /security.txt, so those responses are not genuine\n    endpoints. No API or developer surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reactive-biosciences/refs/heads/main/security/reactive-biosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
