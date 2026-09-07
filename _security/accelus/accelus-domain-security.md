---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_rua: true
  dnssec: false
  domain: accelusinc.com
  mx: accelusinc-com.mail.protection.outlook.com
  nameservers:
  - ns-1193.awsdns-21.org
  - ns-1859.awsdns-40.co.uk
  - ns-864.awsdns-44.net
  note: Mail DNS (Microsoft 365 + HubSpot + Mandrill senders, DMARC p=quarantine) is still in place and the domain registration runs to 2027, but web hosting is suspended and the TLS certificate lapsed on 2026-05-13 — the posture of a wound-down company whose domain registration has simply not yet been dropped. The DMARC rua mailbox is a named individual and is deliberately not recorded here.
  registrar: GoDaddy.com, LLC
  registry_expiry: '2027-06-09'
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:20585452.spf07.hubspotemail.net include:spf.mandrillapp.com ip4:162.217.150.80 -all
hosts:
- cert_expires: '2026-05-13'
  cert_issuer: C=US, O=Let's Encrypt, CN=R13
  cert_not_before: '2026-02-12'
  cert_subject: CN=www.accelusinc.com
  disposition: suspended-hosting-account
  host: accelusinc.com
  hsts: false
  http_redirect: https://accelusinc.com/cgi-sys/suspendedpage.cgi
  http_status: 302
  https: true
  server: LiteSpeed
  tls_cert_error: certificate has expired
  tls_version: TLSv1.3
- disposition: suspended-hosting-account
  host: www.accelusinc.com
  hsts: false
  http_redirect: https://accelusinc.com/cgi-sys/suspendedpage.cgi
  http_status: 302
  https: true
  tls_cert_error: certificate has expired
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Accelus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accelus, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Accelus
provider_slug: accelus
slug: accelus-domain-security
source_filename: accelus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: accelusinc.com (live TLS + DNS probe, 2026-09-06)\nnote: >-\n  Probed by hand rather than by 0-working/probe-domain-security.py: that script collects\n  hosts from Website/Portal pointers and apis[] entries, and accelusinc.com is deliberately\n  NOT wired as a Website pointer because the host is a suspended cPanel account serving an\n  \"Account Suspended\" page on every path (see well-known/accelus-well-known.yml). The\n  values below are what was actually observed.\nhosts:\n- host: accelusinc.com\n  https: true\n  tls_version: TLSv1.3\n  tls_cert_error: certificate has expired\n  cert_issuer: \"C=US, O=Let's Encrypt, CN=R13\"\n  cert_subject: CN=www.accelusinc.com\n  cert_not_before: '2026-02-12'\n  cert_expires: '2026-05-13'\n  hsts: false\n  http_status: 302\n  http_redirect: https://accelusinc.com/cgi-sys/suspendedpage.cgi\n  server: LiteSpeed\n  disposition: suspended-hosting-account\n- host: www.accelusinc.com\n  https:\
  \ true\n  tls_version: TLSv1.3\n  tls_cert_error: certificate has expired\n  hsts: false\n  http_status: 302\n  http_redirect: https://accelusinc.com/cgi-sys/suspendedpage.cgi\n  disposition: suspended-hosting-account\ndomains:\n- domain: accelusinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: \"v=spf1 include:spf.protection.outlook.com include:20585452.spf07.hubspotemail.net include:spf.mandrillapp.com ip4:162.217.150.80 -all\"\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: true\n  mx: accelusinc-com.mail.protection.outlook.com\n  registrar: GoDaddy.com, LLC\n  registry_expiry: '2027-06-09'\n  nameservers:\n  - ns-1193.awsdns-21.org\n  - ns-1859.awsdns-40.co.uk\n  - ns-864.awsdns-44.net\n  note: >-\n    Mail DNS (Microsoft 365 + HubSpot + Mandrill senders, DMARC p=quarantine) is still in\n    place and the domain registration runs to 2027, but web hosting is suspended and the\n    TLS certificate lapsed on 2026-05-13 — the posture of a wound-down company whose\n\
  \    domain registration has simply not yet been dropped. The DMARC rua mailbox is a named\n    individual and is deliberately not recorded here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelus/refs/heads/main/security/accelus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Medical Technology
- Healthcare
- Spine Surgery
- Surgical Robotics
- Implants
- Defunct
---
