

    ██████╗  █████╗ ██╗  ██╗██╗   ██╗██╗      
    ██╔══██╗██╔══██╗██║  ██║██║   ██║██║     
    ██████╔╝███████║███████║██║   ██║██║    
    ██╔══██╗██╔══██║██╔══██║██║   ██║██║     
    ██║  ██║██║  ██║██║  ██║╚██████╔╝███████╗
    ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝ ╚══════╝ 
    

    class Bio {
    constructor() {
    this.aboutMe = {
      name: "Rahul Dadhich",
      description: "Technical Content Writer | Web2 & Web3 Developer",
      status: "Learning Rust, Solidity, and solving DSA problems.",
      goalsFor2024: ["Master Rust & Solidity", "Build advanced Web2 & Web3 projects", "Solve 300+ DSA problems"]
    };
    
    this.workExperience = [
      {
        role: "Technical Content Writer",
        company: "GeeksforGeeks",
        duration: "Current",
        responsibilities: "Write technical articles and tutorials."
      },
      {
        role: "Web2 Developer",
        company: "Self-employed",
        duration: "Ongoing",
        responsibilities: "Build medium to hard-level Web2 projects."
      },
      {
        role: "Web3 Developer",
        company: "Self-taught",
        duration: "Ongoing",
        responsibilities: "Build medium to hard-level Web3 projects."
      }
    ];

    this.tools = {
      frameworks: ["React", "Node.js", "Express"],
      languages: ["JavaScript", "Rust", "Solidity", "C++"],
      databases: ["MongoDB", "Postgres"],
      platforms: ["GNU/Linux", "Windows"],
      otherTools: ["Git", "VS Code", "Truffle", "Hardhat"]
    };

    this.randomStuff = {
      funFact: "I can solve a Rubik's Cube in under 2 minutes!",
      advice: "Keep learning, keep growing, and never stop coding."
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

    const bio = new Bio();
    bio.display();
