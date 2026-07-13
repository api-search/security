---
api_specs:
- filename: vagrant-cloud-api-openapi.yml
  format: yaml
  label: Vagrant Cloud API
  slug: vagrant-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagrant/refs/heads/main/openapi/vagrant-cloud-api-openapi.yml
- filename: vagrant-hcp-vagrant-box-registry-openapi.yml
  format: yaml
  label: HCP Vagrant Box Registry API
  slug: vagrant-hcp-box-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagrant/refs/heads/main/openapi/vagrant-hcp-vagrant-box-registry-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hashicorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vagrantup.com
  spf: true
hosts:
- cert_expires: Sep 21 05:45:45 2026 GMT
  host: developer.hashicorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 15:05:20 2026 GMT
  host: www.vagrantup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: app.vagrantup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vagrant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vagrant, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vagrant
provider_slug: vagrant
slug: vagrant-domain-security
source_filename: vagrant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.vagrantup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 15:05:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.vagrantup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hashicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vagrantup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vagrant/refs/heads/main/security/vagrant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DevOps
- Virtualization
- Development Environments
- Boxes
- Cloud
- HashiCorp
- Infrastructure
---
