---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sparrow.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; adkim=r; aspf=r; rua=mailto:REDACTED@trysparrow.com
  dnskey: present
  dnssec: true
  domain: trysparrow.com
  mx: google
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:emsd1.com include:u12511619.wl120.sendgrid.net include:mail.zendesk.com include:39814015.spf07.hubspotemail.net ~all
hosts:
- cert_expires: Oct 23 08:29:29 2026 GMT
  host: sparrow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 13:11:48 2026 GMT
  host: trysparrow.com
  hsts: null
  https: true
  note: 301 redirect host
  tls_version: TLSv1.3
- cert_expires: Oct 23 08:29:29 2026 GMT
  host: app.sparrow.com
  hsts: max-age=0
  https: true
  note: HSTS header present but max-age is zero, which disables it.
  tls_version: TLSv1.3
- cert_expires: Oct 11 13:11:48 2026 GMT
  csp: true
  csp_note: A strict Content-Security-Policy with default-src 'none' is served. It is also the artifact that revealed Sparrow's own origins — api.trysparrow.com, login.trysparrow.com, support.trysparrow.com and uploads.trysparrow.com.
  host: app.trysparrow.com
  hsts: max-age=63072000; includeSubDomains
  https: true
  tls_version: TLSv1.3
  x_frame_options: deny
kind: domain-security
layout: security
method: probed
name: Sparrow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sparrow, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sparrow
provider_slug: sparrow
slug: sparrow-domain-security
source_filename: sparrow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes (probe-domain-security.py plus dig/openssl probes of the additional\n  trysparrow.com hosts named in the app.trysparrow.com Content-Security-Policy).\nnote: >-\n  Sparrow runs two domains. trysparrow.com is the original operating domain and still carries the\n  application, the API backend, sign-in, support and status; sparrow.com is the newer marketing\n  domain. The security posture differs sharply between them: trysparrow.com is DNSSEC-signed and has\n  both SPF and a DMARC policy at p=quarantine, while sparrow.com has no SPF, no DMARC and no DNSKEY.\n  Neither domain publishes a CAA record. HSTS is enforced on app.trysparrow.com\n  (max-age=63072000; includeSubDomains) but explicitly disabled on app.sparrow.com (max-age=0).\nhosts:\n- host: sparrow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 08:29:29 2026 GMT\n  hsts: null\n- host: trysparrow.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Oct 11 13:11:48 2026 GMT\n  hsts: null\n  note: 301 redirect host\n- host: app.sparrow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 08:29:29 2026 GMT\n  hsts: 'max-age=0'\n  note: HSTS header present but max-age is zero, which disables it.\n- host: app.trysparrow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:11:48 2026 GMT\n  hsts: 'max-age=63072000; includeSubDomains'\n  x_frame_options: deny\n  csp: true\n  csp_note: >-\n    A strict Content-Security-Policy with default-src 'none' is served. It is also the artifact that\n    revealed Sparrow's own origins — api.trysparrow.com, login.trysparrow.com, support.trysparrow.com\n    and uploads.trysparrow.com.\ndomains:\n- domain: sparrow.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: trysparrow.com\n  dnssec: true\n  dnskey: present\n  caa: []\n  spf: true\n  spf_record: >-\n    v=spf1 include:_spf.google.com include:emsd1.com include:u12511619.wl120.sendgrid.net\n\
  \    include:mail.zendesk.com include:39814015.spf07.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; adkim=r; aspf=r; rua=mailto:REDACTED@trysparrow.com'\n  mx: google\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparrow/refs/heads/main/security/sparrow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Leave Management
- Human Resources
- HR Tech
- Payroll
- Compliance
- Employee Benefits
- Absence Management
- Software-as-a-Service
---
