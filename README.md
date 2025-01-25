
    class Bio {
    constructor() {
    this.aboutMe = {
      name: "Rahul Dadhich",
      description: "Technical Content Writer at GeeksforGeeks | Web2 & Web3 Developer",
      status: "Learning Rust, Solidity, and solving DSA problems.",
      goals: {
        2024: ["Master Rust & Solidity", "Build advanced Web2 & Web3 projects", "Solve 300+ DSA problems"],
        2025: ["Create many Web2 & Web3 projects", "Explore advanced blockchain concepts"]
      }
    };
    
    this.workExperience = [
      {
        role: "Technical Content Writer",
        company: "GeeksforGeeks",
        duration: "Current",
        responsibilities: [
          "Write technical articles and tutorials.",
          "Research and stay updated with tech trends."
        ]
      },
      {
        role: "Web2 Developer",
        company: "Self-employed",
        duration: "Ongoing",
        responsibilities: [
          "Build medium to hard-level Web2 projects.",
          "Work with React, Node.js, and WebSockets."
        ]
      },
      {
        role: "Web3 Developer",
        company: "Self-taught",
        duration: "Ongoing",
        responsibilities: [
          "Build medium to hard-level Web3 projects.",
          "Learn and work with Solidity, Ethereum, and Rust."
        ]
      }
    ];

    this.skills = {
      languages: ["JavaScript", "Rust", "Solidity", "C++"],
      frameworks: ["React", "Node.js", "Express"],
      tools: ["Git", "VS Code", "Truffle", "Hardhat"]
    };

    this.projects = {
      web2: [
        {
          name: "3D Metaverse Game",
          description: "Real-time multiplayer 3D game using WebSockets and React.",
          tech: ["React", "WebSockets", "Three.js", "Node.js"]
        }
      ],
      web3: [
        {
          name: "Decentralized Exchange",
          description: "WazirX clone for token trading.",
          tech: ["Solidity", "React", "Web3.js", "Ethereum"]
        },
        {
          name: "Token Launchpad",
          description: "Platform for launching new tokens.",
          tech: ["Solidity", "React", "Web3.js", "IPFS"]
        }
      ],
      cpp: [
        {
          name: "Custom Web Server",
          description: "Lightweight web server using C++.",
          tech: ["C++", "Sockets", "HTTP"]
        }
      ]
    };

    this.socialLinks = {
      leetcode: "https://leetcode.com/u/TheGaurdiann/",
      twitter: "https://x.com/Rahul_Dadhich26",
      geeksforgeeks: "https://www.geeksforgeeks.org/user/rahuldadhich26/",
      codingninjas: "https://www.naukri.com/code360/profile/Rahul_dadhich26",
      github: "https://github.com/rahuldadhich",
      portfolio: "https://rahuldadhich.netlify.app/"
    };
    display() {
    console.log("=== About Me ===");
    console.log(`Name: ${this.aboutMe.name}`);
    console.log(`Description: ${this.aboutMe.description}`);
    console.log(`Status: ${this.aboutMe.status}`);
    console.log("Goals 2024:", this.aboutMe.goals[2024].join(", "));
    console.log("Goals 2025:", this.aboutMe.goals[2025].join(", "));
    console.log("\n");
    }
    console.log("=== Work Experience ===");
    this.workExperience.forEach((job, i) => {
      console.log(`${i + 1}. ${job.role} at ${job.company} (${job.duration})`);
      job.responsibilities.forEach((resp, j) => console.log(`   ${j + 1}. ${resp}`));
    });
    console.log("\n");

    console.log("=== Skills ===");
    console.log("Languages:", this.skills.languages.join(", "));
    console.log("Frameworks:", this.skills.frameworks.join(", "));
    console.log("Tools:", this.skills.tools.join(", "));
    console.log("\n");

    console.log("=== Projects ===");
    console.log("Web2:");
    this.projects.web2.forEach((proj, i) => {
      console.log(`${i + 1}. ${proj.name}: ${proj.description}`);
      console.log("   Tech:", proj.tech.join(", "));
    });

    console.log("Web3:");
    this.projects.web3.forEach((proj, i) => {
      console.log(`${i + 1}. ${proj.name}: ${proj.description}`);
      console.log("   Tech:", proj.tech.join(", "));
    });

    console.log("C++:");
    this.projects.cpp.forEach((proj, i) => {
      console.log(`${i + 1}. ${proj.name}: ${proj.description}`);
      console.log("   Tech:", proj.tech.join(", "));
    });
    console.log("\n");

    console.log("=== Social Links ===");
    for (const [platform, link] of Object.entries(this.socialLinks)) {
      console.log(`${platform}: ${link}`);
    }
    }
    }

    const bio = new Bio();
    bio.display();
