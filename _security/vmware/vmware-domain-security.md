---
api_specs:
- filename: vmware-clusters-api-openapi.yml
  format: yaml
  label: VMware Clusters API
  slug: vmware-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-clusters-api-openapi.yml
- filename: vmware-content-library-api-openapi.yml
  format: yaml
  label: VMware Content Library API
  slug: vmware-content-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-content-library-api-openapi.yml
- filename: vmware-datacenters-api-openapi.yml
  format: yaml
  label: VMware Datacenters API
  slug: vmware-datacenters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-datacenters-api-openapi.yml
- filename: vmware-datastores-api-openapi.yml
  format: yaml
  label: VMware Datastores API
  slug: vmware-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-datastores-api-openapi.yml
- filename: vmware-folders-api-openapi.yml
  format: yaml
  label: VMware Folders API
  slug: vmware-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-folders-api-openapi.yml
- filename: vmware-hosts-api-openapi.yml
  format: yaml
  label: VMware Hosts API
  slug: vmware-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-hosts-api-openapi.yml
- filename: vmware-networks-api-openapi.yml
  format: yaml
  label: VMware Networks API
  slug: vmware-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-networks-api-openapi.yml
- filename: vmware-resource-pools-api-openapi.yml
  format: yaml
  label: VMware Resource Pools API
  slug: vmware-resource-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-resource-pools-api-openapi.yml
- filename: vmware-session-api-openapi.yml
  format: yaml
  label: VMware Session API
  slug: vmware-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-session-api-openapi.yml
- filename: vmware-storage-policies-api-openapi.yml
  format: yaml
  label: VMware Storage Policies API
  slug: vmware-storage-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-storage-policies-api-openapi.yml
- filename: vmware-tagging-api-openapi.yml
  format: yaml
  label: VMware Tagging API
  slug: vmware-tagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-tagging-api-openapi.yml
- filename: vmware-vm-guest-api-openapi.yml
  format: yaml
  label: VMware VM Guest API
  slug: vmware-vm-guest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vm-guest-api-openapi.yml
- filename: vmware-vm-hardware-api-openapi.yml
  format: yaml
  label: VMware VM Hardware API
  slug: vmware-vm-hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vm-hardware-api-openapi.yml
- filename: vmware-vm-power-api-openapi.yml
  format: yaml
  label: VMware VM Power API
  slug: vmware-vm-power-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vm-power-api-openapi.yml
- filename: vmware-vms-api-openapi.yml
  format: yaml
  label: VMware VMs API
  slug: vmware-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: broadcom.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "entrust.net"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vmware.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: developer.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: developer.vmware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: vmc.vmware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vmware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VMware, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: VMware
provider_slug: vmware
slug: vmware-domain-security
source_filename: vmware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.vmware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vmc.vmware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: broadcom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vmware.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/security/vmware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
---
