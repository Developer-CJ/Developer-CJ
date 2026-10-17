# `Christopher.Knapchuck.cs`

```text
╔════════════════════════════════════════════════════════════╗
║                 CJIT SOLUTIONS // PROFILE                  ║
║                 Infrastructure Done Right.                 ║
║                                                            ║
║  [SYSTEM] Developer profile initialized!                   ║
║  [SYSTEM] Connecting to CJIT Mainframe....                 ║
║  [STATUS] ONLINE                                           ║
║  [MODE]   BUILD • AUTOMATE • DEPLOY • SUPPORT              ║
╚════════════════════════════════════════════════════════════╝
```

```csharp
using System;
using System.Collections.Generic;
using System.Linq;

namespace CJIT.Solutions;

public static class DeveloperProfile
{
    public static void Main()
    {
        var chris = new Engineer
        {
            Name = "Christopher J. Knapchuck",
            Alias = "CJ",
            Location = "Michigan, USA",
            Company = "CJIT Solutions",
            Position = "Founder | Network & Software Engineer",
            Education = "Self-Taught | Hands-On Experience",
            Philosophy = "Plan. Test. Deliver. Support.",
            Status = "Building the next generation of IT infrastructure"
        };

        Console.WriteLine("Initializing CJIT Developer Environment...");
        Console.WriteLine("Loading professional identity...");
        Console.WriteLine();

        chris.Introduce();
        chris.DisplaySkills();
        chris.DisplayInfrastructure();
        chris.DisplayProjects();
        chris.DisplayMission();

        Console.WriteLine("\n[✓] Profile loaded successfully.");
        Console.WriteLine("[✓] Innovation engine operational.");
        Console.WriteLine("[>] Awaiting next challenge...");
    }
}

public class Engineer
{
    public string Name { get; init; } = "";
    public string Alias { get; init; } = "";
    public string Location { get; init; } = "";
    public string Company { get; init; } = "";
    public string Position { get; init; } = "";
    public string Education { get; init; } = "";
    public string Philosophy { get; init; } = "";
    public string Status { get; init; } = "";

    private readonly Dictionary<string, string[]> _skills = new()
    {
        ["Software Engineering"] = new[]
        {
            "C#", ".NET", "Python", "PowerShell",
            "C++", "JavaScript", "SQL"
        },

        ["Systems Administration"] = new[]
        {
            "Windows Server", "Active Directory",
            "DNS", "DHCP", "Group Policy",
            "Linux", "Virtualization"
        },

        ["Networking & Security"] = new[]
        {
            "TCP/IP", "Routing & Switching",
            "Firewalls", "VPN", "Zero Trust",
            "Network Troubleshooting"
        },

        ["Cloud & Infrastructure"] = new[]
        {
            "Cloudflare Workers", "Cloudflare D1",
            "Cloudflare R2", "AWS",
            "Proxmox", "VMware", "Hyper-V"
        },

        ["Business Technology"] = new[]
        {
            "Managed IT Services", "Retail POS",
            "CCTV / NVR", "Remote Support",
            "Web Hosting", "Infrastructure Monitoring"
        }
    };

    public void Introduce()
    {
        Console.WriteLine($"Name       : {Name}");
        Console.WriteLine($"Known As   : {Alias}");
        Console.WriteLine($"Location   : {Location}");
        Console.WriteLine($"Company    : {Company}");
        Console.WriteLine($"Role       : {Position}");
        Console.WriteLine($"Background : {Education}");
        Console.WriteLine($"Status     : {Status}");
    }

    public void DisplaySkills()
    {
        Console.WriteLine("\n[LOADING TECHNICAL CAPABILITIES]");

        foreach (var category in _skills)
        {
            Console.WriteLine($"\n> {category.Key}");

            foreach (var technology in category.Value)
                Console.WriteLine($"  [+] {technology}");
        }
    }

    public void DisplayInfrastructure()
    {
        Console.WriteLine("\n[INFRASTRUCTURE ENVIRONMENT]");

        string[] infrastructure =
        {
            "Windows Server & Active Directory",
            "Proxmox / VMware / Hyper-V",
            "Cloudflare Workers / D1 / R2",
            "Hybrid Cloud & Self-Hosted Services",
            "Network Monitoring & Remote Management",
            "Custom Internal Business Applications"
        };

        foreach (var system in infrastructure)
            Console.WriteLine($"[READY] {system}");
    }

    public void DisplayProjects()
    {
        Console.WriteLine("\n[PROJECT REGISTRY]");

        var projects = new[]
        {
            "CJIT Mainframe",
            "CJIT Commerce",
            "CJIT RadioLink",
            "CJIT ProjectHub Ops",
            "CJIT AI Mission Control",
            "CJIT Neural Network Visualizer",
            "PetroCore POS",
            "CJIT Client Services Portal"
        };

        foreach (var project in projects)
            Console.WriteLine($"[PROJECT] {project}");
    }

    public void DisplayMission()
    {
        Console.WriteLine("\n[MISSION STATEMENT]");
        Console.WriteLine(
            "Transform complex infrastructure into practical, " +
            "reliable and maintainable technology solutions."
        );

        Console.WriteLine($"\n[OPERATING PRINCIPLE] {Philosophy}");
    }
}
```

## `dotnet run` — Console Output

```console
PS C:\CJIT\Profile> dotnet run

Initializing CJIT Developer Environment...
Loading professional identity...

Name       : Christopher J. Knapchuck
Known As   : CJ
Location   : Michigan, USA
Company    : CJIT Solutions
Role       : Founder | Network & Software Engineer
Background : Self-Taught | Hands-On Experience
Status     : Building the next generation of IT infrastructure

[LOADING TECHNICAL CAPABILITIES]

> Software Engineering
  [+] C#
  [+] .NET
  [+] Python
  [+] PowerShell
  [+] C++
  [+] JavaScript
  [+] SQL

> Systems Administration
  [+] Windows Server
  [+] Active Directory
  [+] DNS
  [+] DHCP
  [+] Group Policy
  [+] Linux
  [+] Virtualization

> Networking & Security
  [+] TCP/IP
  [+] Routing & Switching
  [+] Firewalls
  [+] VPN
  [+] Zero Trust
  [+] Network Troubleshooting

> Cloud & Infrastructure
  [+] Cloudflare Workers
  [+] Cloudflare D1
  [+] Cloudflare R2
  [+] AWS
  [+] Proxmox
  [+] VMware
  [+] Hyper-V

> Business Technology
  [+] Managed IT Services
  [+] Retail POS
  [+] CCTV / NVR
  [+] Remote Support
  [+] Web Hosting
  [+] Infrastructure Monitoring

[INFRASTRUCTURE ENVIRONMENT]
[READY] Windows Server & Active Directory
[READY] Proxmox / VMware / Hyper-V
[READY] Cloudflare Workers / D1 / R2
[READY] Hybrid Cloud & Self-Hosted Services
[READY] Network Monitoring & Remote Management
[READY] Custom Internal Business Applications

[PROJECT REGISTRY]
[PROJECT] CJIT Mainframe
[PROJECT] CJIT Commerce
[PROJECT] CJIT RadioLink
[PROJECT] CJIT ProjectHub Ops
[PROJECT] CJIT AI Mission Control
[PROJECT] CJIT Neural Network Visualizer
[PROJECT] PetroCore POS
[PROJECT] CJIT Client Services Portal

[MISSION STATEMENT]
Transform complex infrastructure into practical,
reliable and maintainable technology solutions.

[OPERATING PRINCIPLE] Plan. Test. Deliver. Support.

[✓] Profile loaded successfully.
[✓] Innovation engine operational.
[>] Awaiting next challenge...
```

---

## `AboutMe.cs`

```csharp
public record AboutMe
{
    public string LearningStyle => "Hands-On";

    public string CareerPath => "Self-Taught Engineer";

    public string PrimaryFocus =>
        "Networking, Software, Cloud & Infrastructure";

    public bool EnjoysSolvingComplexProblems => true;

    public bool BelievesInContinuousLearning => true;

    public bool BuildsRealWorldSolutions => true;

    public string[] CurrentObjectives =>
    [
        "Grow CJIT Solutions",
        "Expand managed infrastructure services",
        "Develop enterprise-inspired software",
        "Build automation-first platforms",
        "Create reliable self-hosted solutions"
    ];
}
```

## `Company.cs`

```csharp
namespace CJIT.Solutions;

public static class Company
{
    public const string Name = "CJIT Solutions";
    public const string Motto = "Infrastructure Done Right.";
    public const string OperatingModel = "Plan. Test. Deliver. Support.";

    public static readonly string[] Services =
    [
        "Managed IT Services",
        "Network Engineering",
        "Software Development",
        "Server Administration",
        "Cloud & Web Hosting",
        "IT Infrastructure Support",
        "Security & Surveillance",
        "Automation & Systems Integration"
    ];

    public static string Website =>
        "https://cjitsystems.com";
}
```

## `DeveloperMindset.cs`

```csharp
while (true)
{
    Learn();
    Experiment();
    Build();
    Test();
    Improve();
    Deploy();

    // Every solution creates an opportunity
    // to engineer something even better.
}
```

## `Connect.cs`

```csharp
Console.WriteLine("Interested in collaborating?");
Console.WriteLine("Company: CJIT Solutions");
Console.WriteLine("Website: https://cjitsystems.com");
Console.WriteLine("Focus: Software | Networks | Cloud | IT");
Console.WriteLine("Status: Open to technical collaboration");
```

**[CJIT Solutions](https://cjitsystems.com)**

---

```console
┌─────────────────────────────────────────────────────────┐
│ CJIT SOLUTIONS                                          │
│                                                         │
│ Infrastructure Done Right.                              │
│ Plan. Test. Deliver. Support.                           │
│                                                         │
│ System Status: OPERATIONAL                              │
│ Engineering Mindset: ALWAYS ACTIVE                      │
│ Next Objective: BUILD SOMETHING BETTER                  │
└─────────────────────────────────────────────────────────┘
```
