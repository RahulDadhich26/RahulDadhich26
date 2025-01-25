class Bio {
  constructor() {
    this.aboutMe = {
      name: "Rahul Dadhich",
      description: "Technical Content Writer at GeeksforGeeks | Web2 and Web3 Developer",
      status: "Living my best life, learning Rust, Solidity, and solving DSA problems.",
      goalsFor2024: [
        "Master Rust and Solidity.",
        "Build advanced Web2 and Web3 projects.",
        "Solve 300+ DSA problems.",
        "Contribute to open-source projects."
      ],
      goalsFor2025: [
        "Create a lot of projects in Web2 and Web3.",
        "Explore advanced blockchain concepts.",
        "Publish technical articles and tutorials."
      ]
    };

    this.workExperience = [
      {
        role: "Technical Content Writer",
        company: "GeeksforGeeks",
        duration: "Current",
        responsibilities: [
          "Writing high-quality technical articles on programming and development.",
          "Creating tutorials and guides for developers.",
          "Researching and staying updated with the latest tech trends."
        ]
      },
      {
        role: "Web2 Developer",
        company: "Self-employed",
        duration: "Ongoing",
        responsibilities: [
          "Building medium to hard-level Web2 projects.",
          "Working with technologies like React, Node.js, and WebSockets.",
          "Creating scalable and user-friendly applications."
        ]
      },
      {
        role: "Web3 Learner and Developer",
        company: "Self-taught",
        duration: "Ongoing",
        responsibilities: [
          "Learning and building medium to hard-level Web3 projects.",
          "Exploring blockchain, smart contracts, and decentralized apps (dApps).",
          "Working with Solidity, Ethereum, and Rust."
        ]
      }
    ];

    this.skills = {
      programmingLanguages: ["JavaScript", "Rust", "Solidity", "C++"],
      frameworks: ["React", "Node.js", "Express"],
      tools: ["Git", "VS Code", "Truffle", "Hardhat"],
      platforms: ["GeeksforGeeks", "LeetCode", "HackerRank"],
      interests: ["Web Development", "Blockchain", "Technical Writing", "Problem Solving"]
    };

    this.projects = {
      web2: [
        {
          name: "3D Metaverse Game",
          description: "A real-time multiplayer 3D game built using WebSockets and React.",
          technologies: ["React", "WebSockets", "Three.js", "Node.js"],
          features: [
            "Real-time multiplayer interaction.",
            "3D environment rendering using Three.js.",
            "Scalable backend using Node.js and WebSockets."
          ]
        }
      ],
      web3: [
        {
          name: "Decentralized Exchange (WazirX Clone)",
          description: "A decentralized exchange inspired by WazirX, built using Web3 technologies.",
          technologies: ["Solidity", "React", "Web3.js", "Ethereum"],
          features: [
            "Token trading and swapping.",
            "Integration with Ethereum blockchain.",
            "User-friendly interface for trading."
          ]
        },
        {
          name: "Token Launchpad",
          description: "A platform for launching new tokens and conducting ICOs.",
          technologies: ["Solidity", "React", "Web3.js", "IPFS"],
          features: [
            "Token creation and deployment.",
            "Secure ICO participation.",
            "Integration with IPFS for decentralized storage."
          ]
        },
        {
          name: "Wallet Adapter",
          description: "A wallet adapter for connecting multiple blockchain wallets.",
          technologies: ["Web3.js", "Ethereum", "Solana", "WalletConnect"],
          features: [
            "Support for multiple wallets (MetaMask, Phantom, etc.).",
            "Easy integration with dApps.",
            "Secure transaction signing."
          ]
        }
      ],
      cpp: [
        {
          name: "Custom Web Server",
          description: "A lightweight web server built from scratch using C++.",
          technologies: ["C++", "Sockets", "HTTP"],
          features: [
            "Handles HTTP GET and POST requests.",
            "Multi-threaded for handling multiple clients.",
            "Custom routing and request handling."
          ]
        }
      ]
    };

    this.randomStuff = {
      funFact: "I can solve a Rubik's Cube in under 2 minutes!",
      advice: "Keep learning, keep growing, and never stop coding.",
      quote: "The best way to predict the future is to create it."
    };

    this.socialLinks = {
      leetcode: "https://leetcode.com/u/TheGaurdiann/",
      twitter: "https://x.com/Rahul_Dadhich26",
      geeksforgeeks: "https://www.geeksforgeeks.org/user/rahuldadhich26/",
      codingninjas: "https://www.naukri.com/code360/profile/Rahul_dadhich26",
      github: "https://github.com/rahuldadhich",
      portfolio: "https://rahuldadhich.netlify.app/"
    };
  }

  display() {
    console.log("=== About Me ===");
    console.log(`Name: ${this.aboutMe.name}`);
    console.log(`Description: ${this.aboutMe.description}`);
    console.log(`Status: ${this.aboutMe.status}`);
    console.log(`Goals for 2024: ${this.aboutMe.goalsFor2024.join(", ")}`);
    console.log(`Goals for 2025: ${this.aboutMe.goalsFor2025.join(", ")}`);
    console.log("\n");

    console.log("=== Work Experience ===");
    this.workExperience.forEach((job, index) => {
      console.log(`Job ${index + 1}:`);
      console.log(`Role: ${job.role}`);
      console.log(`Company: ${job.company}`);
      console.log(`Duration: ${job.duration}`);
      console.log(`Responsibilities:`);
      job.responsibilities.forEach((resp, i) => console.log(`  ${i + 1}. ${resp}`));
      console.log("\n");
    });

    console.log("=== Skills ===");
    console.log(`Programming Languages: ${this.skills.programmingLanguages.join(", ")}`);
    console.log(`Frameworks: ${this.skills.frameworks.join(", ")}`);
    console.log(`Tools: ${this.skills.tools.join(", ")}`);
    console.log(`Platforms: ${this.skills.platforms.join(", ")}`);
    console.log(`Interests: ${this.skills.interests.join(", ")}`);
    console.log("\n");

    console.log("=== Projects ===");
    console.log("Web2 Projects:");
    this.projects.web2.forEach((project, index) => {
      console.log(`Project ${index + 1}:`);
      console.log(`Name: ${project.name}`);
      console.log(`Description: ${project.description}`);
      console.log(`Technologies: ${project.technologies.join(", ")}`);
      console.log(`Features:`);
      project.features.forEach((feature, i) => console.log(`  ${i + 1}. ${feature}`));
      console.log("\n");
    });

    console.log("Web3 Projects:");
    this.projects.web3.forEach((project, index) => {
      console.log(`Project ${index + 1}:`);
      console.log(`Name: ${project.name}`);
      console.log(`Description: ${project.description}`);
      console.log(`Technologies: ${project.technologies.join(", ")}`);
      console.log(`Features:`);
      project.features.forEach((feature, i) => console.log(`  ${i + 1}. ${feature}`));
      console.log("\n");
    });

    console.log("C++ Projects:");
    this.projects.cpp.forEach((project, index) => {
      console.log(`Project ${index + 1}:`);
      console.log(`Name: ${project.name}`);
      console.log(`Description: ${project.description}`);
      console.log(`Technologies: ${project.technologies.join(", ")}`);
      console.log(`Features:`);
      project.features.forEach((feature, i) => console.log(`  ${i + 1}. ${feature}`));
      console.log("\n");
    });

    console.log("=== Random Stuff ===");
    console.log(`Fun Fact: ${this.randomStuff.funFact}`);
    console.log(`Advice: ${this.randomStuff.advice}`);
    console.log(`Quote: ${this.randomStuff.quote}`);
    console.log("\n");

    console.log("=== Social Links ===");
    for (const [platform, link] of Object.entries(this.socialLinks)) {
      console.log(`${platform.charAt(0).toUpperCase() + platform.slice(1)}: ${link}`);
    }
  }
}

const bio = new Bio();
bio.display(); 
