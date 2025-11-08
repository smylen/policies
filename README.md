# Smylen HIPAA Compliance Policies

HIPAA compliance is complicated, but it doesn't have to be. Smylen forked the Datica policies to help relieve the technical burden with our HIPAA-compliant platform and solutions for healthcare.

## Why did we use open source policies?

HIPAA compliance really has two halves. The first half includes all technical guidelines, both physical and digital. Compliant companies take measures to secure their hardware and manage their software in a certain way. Encryption, logging, monitoring—these are just a few examples of HIPAA technical requirements. Smylen builds its platform with these guidelines in mind.

The second half of HIPAA is focused on administrative and organizational activities. This includes signing Business Associate Agreements (BAAs), and managing company policies like training, among other things. Crafting company policies that align with HIPAA administrative guidelines are straightforward, but an immense burden.

By using open source policies, we who handle PHI, will benefit.

## What do I do with these policies?

As a company who handles PHI, it's critical you maintain and publish your own policies. To make use of our policies, we recommend the following steps.

[x] Read through all the enclosed policies to get an understanding to the structure.
[x] When ready, download the policies and comb through for mentions of Smylen or our business and change to appropriate references to your company.
[] Publish your policies in a publicly available location. The files are markdown, so you may need to convert to HTML if you don't have a publishing platform capable of markdown format. You can either create an index page linking to each individual policy, or create a single page listing all the policies in line, [much like we did](https://security-policy.smylen.com).

## Who is behind this?

[Smylen](htts://smylen.com), a marketplace with the mission to make dental care accessible by everybody.

To get in touch, shoot us an email at [hello@smylen.com](mailto:hello@smylen.com). We'd love to hear from you!

### License

All policies are licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).

### Policy Index

Each policy is included as its own markdown file in case you want to cherry-pick specific policies. If you currently have no policies in place, we encourage you to consider utilizing all compliance policies.

* [Introduction](docs/01-introduction.md)
* [HIPAA Inheritance](docs/02-hipaa_inheritance.md)
* [Policy Management Policy](docs/03-policy_management_policy.md)
* [Risk Management Policy](docs/04-risk_management_policy.md)
* [Roles Policy](docs/05-roles_policy.md)
* [Data Management Policy](docs/06-data_management_policy.md)
* [System Access Policy](docs/07-systems_access_policy.md)
* [Auditing Policy](docs/08-auditing_policy.md)
* [Configuration Management Policy](docs/09-configuration_management_policy.md)
* [Facility Access Policy](docs/10-facility_access_policy.md)
* [Incident Response Policy](docs/11-incident_response_policy.md)
* [Breach Policy](docs/12-breach_policy.md)
* [Disaster Recovery Policy](docs/13-disaster_recovery_policy.md)
* [Disposable Media Policy](docs/14-disposable_media_policy.md)
* [IDS Policy](docs/15-ids_policy.md)
* [Vulnerability Scanning Policy](docs/16-vulnerability_scanning_policy.md)
* [Data Integrity Policy](docs/17-data_integrity_policy.md)
* [Data Retention Policy](docs/18-data_retention_policy.md)
* [Employees Policy](docs/19-employees_policy.md)
* [Approved Tools Policy](docs/20-approved_tools_policy.md)
* [3rd Party Policy](docs/21-3rd_party_policy.md)
* [Key Definitions](docs/22-key_definitions.md)
* [Smylen HIPAA Business Associate Agreement (“BAA”)](docs/23-smylen_hipaa_business_associate_agreement.md)
* [HIPAA Mappings to Smylen Controls](docs/24-hipaa_mapping_to_smylen_controls.md)

### Developing

Run the following command in your terminal to setup the project:

```bash
scripts/install
```

This will install the project into a virtual environment which you can activate with `source .venv/bin/activate`.

Once you've activated your virtual environment, you can run the site locally:

```bash
mkdocs serve --livereload
```

The site will served on <http://127.0.0.1:8000>.
