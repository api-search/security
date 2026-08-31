---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: educ-up.fr
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: domissori.fr
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edacademy.fr
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: educ-up.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 09:59:21 2026 GMT
  host: domissori.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 15:24:28 2026 GMT
  host: www.edacademy.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 08:11:38 2026 GMT
  host: formation.edacademy.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Educ Up Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Educ-up, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Educ-up
provider_slug: educ-up
slug: educ-up-domain-security
source_filename: educ-up-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: educ-up.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\n- host: domissori.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 09:59:21 2026 GMT\n  hsts: false\n- host: www.edacademy.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:24:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: formation.edacademy.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 08:11:38 2026 GMT\n  hsts: false\ndomains:\n- domain: educ-up.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: domissori.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: edacademy.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnotes: 'Probed the corporate domain educ-up.fr plus\
  \ the two live brand hosts operated by the group, domissori.fr\n  and www.edacademy.fr, because educ-up.fr no longer serves a site (it 302s to http://s880385942.onlinehome.fr/,\n  an IONOS shared-hosting default page). educ-up.fr still resolves and terminates TLS, so the TLS/DNS\n  posture below is real for the domain even though no content is served. formation.edacademy.fr is also\n  probed: it is the self-hosted Moodle learning-management system Edacademy delivers its online training\n  through (Apache/2.4.58 on Ubuntu, MoodleSession cookie, login gate at /login/index.php).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/educ-up/refs/heads/main/security/educ-up-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Edtech
- Education
- Childcare
- Training
- Montessori
- Vocational Training
- France
- Social Impact
---
