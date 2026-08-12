---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: capsovision.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; rua=mailto:dmarc@capsovision.com; adkim=s; aspf=s
  dnssec: false
  domain: capsocloud.com
  spf: false
hosts:
- cert_expires: Sep 13 07:56:36 2026 GMT
  host: capsovision.com
  hsts: false
  https: true
  note: every path answers HTTP 202 with a SiteGround captcha challenge (sg-captcha; header)
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  cert_subject: CN=*.capsocloud.com
  host: www.capsocloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: investors.capsovision.com
  http_status: 403
  https: true
  note: Akamai-fronted Q4/gcs-web investor site; blocks automated clients
  reachable: false
kind: domain-security
layout: security
method: probed
name: Capsovision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CapsoVision, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CapsoVision
provider_slug: capsovision
slug: capsovision-domain-security
source_filename: capsovision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the apis.yml Website + Login hosts\nnote: >-\n  Two hosts carry CapsoVision's public surface: the WordPress marketing site at\n  capsovision.com and the CapsoCloud clinical web application at www.capsocloud.com.\n  Neither serves HSTS and neither publishes a CAA record. capsocloud.com has no SPF\n  record of its own and no DNSSEC, but does publish a strict DMARC reject policy that\n  reports to dmarc@capsovision.com. The investor-relations host\n  investors.capsovision.com (Akamai / gcs-web.com) answered HTTP 403 to every\n  automated request and could not be probed.\nhosts:\n- host: capsovision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:56:36 2026 GMT\n  hsts: false\n  note: every path answers HTTP 202 with a SiteGround captcha challenge (sg-captcha; header)\n- host: www.capsocloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  cert_subject:\
  \ CN=*.capsocloud.com\n  hsts: false\n- host: investors.capsovision.com\n  https: true\n  reachable: false\n  http_status: 403\n  note: Akamai-fronted Q4/gcs-web investor site; blocks automated clients\ndomains:\n- domain: capsovision.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: capsocloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: 'v=DMARC1; p=reject; rua=mailto:dmarc@capsovision.com; adkim=s; aspf=s'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capsovision/refs/heads/main/security/capsovision-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Capsule Endoscopy
- Gastroenterology
- Medical Imaging
- Artificial Intelligence
- Cloud Software
---
