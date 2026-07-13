---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: emailjs.com
  spf: true
hosts:
- cert_expires: Aug 22 09:41:02 2026 GMT
  host: www.emailjs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emailjs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmailJS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EmailJS
provider_slug: emailjs
slug: emailjs-domain-security
source_filename: emailjs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emailjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 09:41:02 2026 GMT\n  hsts: false\ndomains:\n- domain: emailjs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailjs/refs/heads/main/security/emailjs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Email
- Public APIs
---
