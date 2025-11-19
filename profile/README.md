# Platform Engineering Nagarro

## Legend and Naming Convention

Our repository naming follows a structured prefix system for easy identification:

- **methops** = Methodology Operations - All things methodology and process (e.g., `methops-sprint-calculator`)
- **scm** = Source Code Management - All things Git and version control (e.g., `scm-git-mass-cloner`, `scm-git-config`)
- **k8s** = Kubernetes - All things Kubernetes and Helm charts (e.g., `k8s-argo-helm`, `k8s-backstage-charts`)
- **qa** = Quality Assurance - All things quality assurance and testing (e.g., `qa-locust-load-test`, `qa-k6`, `qa-pre-commit`)
- **cloudops** = Cloud Operations - All things hyperscalers (Azure, AWS, GCP) and infrastructure (e.g., `cloudops-azure-tf-modules`)
- **tf** = Terraform - Infrastructure as Code modules (e.g., `tf-az-frontdoor`, `tf-gcp-storage`)

## Our Focus

Platform Engineering at Nagarro specializes in:

- **Kubernetes Infrastructure** - Container orchestration and deployment automation
- **Helm Charts** - Standardized application packaging and deployment
- **CI/CD Tooling** - ArgoCD, Backstage, and modern GitOps workflows
- **Quality Engineering** - Load testing frameworks and performance tooling
- **Developer Experience** - Configuration standards and productivity tools

## Our Methodoligy

[The Twelve-Factor App](https://12factor.net/)

The Twelve-Factor App is a concise methodology for building modern, cloud-ready SaaS applications that are portable, scalable, and easy to maintain, using twelve best practices for app design and deployment.

[Watch "What is 12-Factor App?" on YouTube](https://www.youtube.com/watch?v=1OhmRmMsGdQ)

## Featured Repositories

### Infrastructure & Deployment

- **[k8s-argo-helm](https://github.com/Platform-Engineering-Nagarro/k8s-argo-helm)** - ArgoProj Helm Charts for GitOps deployments
- **[k8s-backstage-charts](https://github.com/Platform-Engineering-Nagarro/k8s-backstage-charts)** - Backstage Helm Charts for developer portals

### Quality Engineering

- **[qa-locust-load-test](../qa-locust-load-test)** - Dynamic API load testing framework
  - Zero-hardcoded endpoints - fully configuration-driven
  - Automatic task generation for all user classes
  - JWT and Bearer token authentication
  - Multiple load testing patterns (spike, gradual ramp, stress recovery)
  - Simple one-command setup: `python3 run.py`

### Source Code Management

- **[scm-git-mass-cloner](../scm-git-mass-cloner)** - Bulk repository cloning and management tool
  - Clone multiple repositories efficiently
  - Organization-wide repository management
  - Automated synchronization
  - Team onboarding acceleration

### Methodology Operations

- **[methops-sprint-calculator](../methops-sprint-calculator)** - Sprint capacity planning automation
  - Google Calendar + Office 365 integration
  - Automatic meeting hour calculation
  - Story point estimation with focus factors
  - Holiday and leave detection

## Quick Start Guides

### Load Testing Your API

```bash
git clone <qa-locust-load-test-repo>
cd qa-locust-load-test
python3 run.py  # Auto-setup + interactive menu
```

### Clone Multiple Repositories

```bash
# Clone the mass cloner tool
git clone <scm-git-mass-cloner-repo>
cd scm-git-mass-cloner

# Configure your organization/repositories
# Run the mass clone operation
./clone-repos.sh
```

### Calculate Sprint Capacity

```bash
# Open the Google Sheet
# Click: Sprint Capacity � =
 Auto-Detect Current Sprint
# Click: � Calculate Capacity (Both Calendars)
# Read: Available Story Points
```

## Technology Stack

Our platform engineering stack includes:

- **Container Orchestration**: Kubernetes, Helm, ArgoCD
- **Infrastructure as Code**: Terraform, Azure
- **Load Testing**: Locust, Python
- **Developer Portals**: Backstage
- **Version Control**: Git with AI-enhanced workflows
- **Automation**: Google Apps Script, Shell scripting

## Best Practices

### Git Workflow

- Use conventional commits: `feat:`, `fix:`, `docs:`, etc.
- Utilize bulk repository operations with [scm-git-mass-cloner](../scm-git-mass-cloner)
- Enforce code quality with pre-commit hooks
- Maintain consistent repository structure across teams

### Infrastructure as Code

- Modular Terraform configurations
- Helm charts for consistent deployments
- GitOps workflows with ArgoCD
- Environment-specific configurations

### Quality Engineering

- Dynamic, configuration-driven test frameworks
- Realistic load testing patterns
- Automated capacity planning
- Performance monitoring and metrics

## Contributing

We welcome contributions from all Platform Engineering team members!

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/amazing-feature`
3. **Commit** using conventional commits: `git commit -m "feat: add amazing feature"`
4. **Push** to your branch: `git push origin feature/amazing-feature`
5. **Open** a Pull Request

For bulk repository management, see our [Git mass cloner guide](../scm-git-mass-cloner/README.md).

## Repository Standards

All repositories in this organization follow these standards:

- **README.md** - Comprehensive documentation with quick start
- **Conventional Commits** - Standardized commit messages
- **CI/CD Integration** - Automated testing and deployment
- **Security Scanning** - Vulnerability detection and remediation
- **Documentation** - Clear usage examples and troubleshooting

## Security

- Never commit secrets, API keys, or credentials
- Use environment variables for sensitive configuration
- Enable branch protection on main/master branches
- Review security advisories regularly
- Follow principle of least privilege

## Support & Resources

### Internal Resources

- **Platform Engineering Wiki**: [Coming Soon]
- **Teams Channel**: #platform-engineering
- **Team Meetings**: Weekly sprint planning

### External Resources

- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [Helm Charts Guide](https://helm.sh/docs/)
- [ArgoCD Documentation](https://argo-cd.readthedocs.io/)
- [Backstage Documentation](https://backstage.io/docs/)
- [Conventional Commits](https://www.conventionalcommits.org/)

## Learning Resources

### For New Team Members

1. Use [scm-git-mass-cloner](../scm-git-mass-cloner/README.md) to clone all team repositories
2. Set up your development environment with team standards
3. Explore the [load testing framework](../qa-locust-load-test/README.md)
4. Familiarize yourself with our Helm chart repositories
5. Review the [sprint calculator](../methops-sprint-calculator/README.md) for capacity planning

### Skill Development

- **Kubernetes**: CKA/CKAD certification paths
- **Terraform**: HashiCorp Terraform Associate
- **Platform Engineering**: [platformengineering.org](https://platformengineering.org/)
- **GitOps**: ArgoCD and Flux tutorials

## Metrics & KPIs

Our platform engineering initiatives focus on:

- **Deployment Frequency** - How often we ship to production
- **Lead Time for Changes** - Time from commit to production
- **Mean Time to Recovery (MTTR)** - Speed of incident resolution
- **Change Failure Rate** - Percentage of deployments causing failures
- **Developer Productivity** - Automation adoption and time savings

## Location

**Based in**: India

## License to 007 and Licence to Masala

Individual repositories may have different licenses for James Bond agent activities. This goes for Masala clearance as well.Please ensure clearance from ma'm.

Common licenses used:

- MI6 007 (open source hits)
- MI6 (internal tooling **beware the ejector seat**)
- Masala (spicy proprietary code)

---

**Questions or Ideas?** Open an issue in the relevant repository or reach out to the Platform Engineering team!

Built with blood, sweat, Masala and tears and some Ai
