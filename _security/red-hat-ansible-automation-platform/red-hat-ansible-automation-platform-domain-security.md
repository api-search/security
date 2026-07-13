---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:it-cert-admin@redhat.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redhat.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.redhat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: access.redhat.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Red Hat Ansible Automation Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Hat Ansible Automation Platform, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Red Hat Ansible Automation Platform
provider_slug: red-hat-ansible-automation-platform
slug: red-hat-ansible-automation-platform-domain-security
source_filename: red-hat-ansible-automation-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: access.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: redhat.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:it-cert-admin@redhat.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/security/red-hat-ansible-automation-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Configuration Management
- DevOps
- Enterprise
- Red Hat
---
