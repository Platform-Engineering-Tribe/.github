# Platform Engineering Nagarro

> The home of Platform Engineering

Welcome to the Platform Engineering Nagarro GitHub organization - your central hub for infrastructure tooling, automation frameworks, and development best practices.

## Our Focus

Platform Engineering at Nagarro specializes in:

- **Kubernetes Infrastructure** - Container orchestration and deployment automation
- **Helm Charts** - Standardized application packaging and deployment
- **CI/CD Tooling** - ArgoCD, Backstage, and modern GitOps workflows
- **Quality Engineering** - Load testing frameworks and performance tooling
- **Developer Experience** - Configuration standards and productivity tools

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

### Azure Infrastructure

- **[az-tf-frontdoor](../az-tf-frontdoor)** - Azure Front Door Terraform modules
  - Enterprise-grade Azure CDN and load balancing
  - Infrastructure as Code for global traffic management

### Developer Tooling

- **[scm-git-config](../scm-git-config)** - Git configuration standards and best practices
  - AI-powered commit message generation (Gemini)
  - Conventional commit enforcement
  - VS Code / Cursor integration
  - Enhanced diff tools (Delta)
  - Team-wide configuration scripts

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

### Standardize Git Configuration

```bash
# Download team Git setup script
curl -o team-git-setup.sh <scm-git-config-repo>/team-git-setup.sh
chmod +x team-git-setup.sh
./team-git-setup.sh
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
- Leverage AI-powered commit messages (see [scm-git-config](../scm-git-config))
- Enforce code quality with pre-commit hooks
- Generate comprehensive PR descriptions automatically

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

For AI-powered commits, see our [Git configuration guide](../scm-git-config/README.md).

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
- **Slack Channel**: #platform-engineering
- **Team Meetings**: Weekly sprint planning

### External Resources

- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [Helm Charts Guide](https://helm.sh/docs/)
- [ArgoCD Documentation](https://argo-cd.readthedocs.io/)
- [Backstage Documentation](https://backstage.io/docs/)
- [Conventional Commits](https://www.conventionalcommits.org/)

## Learning Resources

### For New Team Members

1. Review our [Git configuration standards](../scm-git-config/README.md)
2. Set up your development environment with team configs
3. Explore the [load testing framework](../qa-locust-load-test/README.md)
4. Familiarize yourself with our Helm chart repositories

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

Individual repositories may have different licenses for James agent activities.
Please ensure clearance from ma'm.

Common licenses used:

- MI6 007 (open source hits)
- MI6 (internal tooling **beware the ejector seat**)
- Masala (spicy proprietary code)

---

**Questions or Ideas?** Open an issue in the relevant repository or reach out to the Platform Engineering team!

Built with blood, sweat, Masala and tears and some Ai
