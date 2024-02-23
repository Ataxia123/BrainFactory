export type HackathonEntry = {
    address: string;
    _id: string;
    hack: HackathonProjectAttributes;
    teamMembers: TeamMember[];
    eval: AIEvaluation[];
    progressUpdates: ProgressUpdate[];
};

// Team Member
export type TeamMember = {
    name: string;
    email: string;
    role: string;
};

export type CodeEntry = {
    code: string;
    comment: string;
    language: string;
};

export type ProgressUpdate = {
    progress: string;
    wins: string;
    losses: string;
    gamePlan: string;
    actionItems: string[];
    codeSnippets: CodeEntry[];
};

export type HackathonProjectAttributes = {
    projectName: string;
    problemStatement: string;
    solutionDescription: string;
    implementationDescription: string;
    technologyStack: string[];
};

export type AIEvaluation = {
    coherenceScore: number;
    feasibilityScore: number;
    innovationScore: number;
    funScore: number;
    evaluationRemarks: string;
    codeSnippets: CodeEntry[];
}

---
# <u>Assistant</u>

// Example entry for a hackathon
const hackathonEntry: HackathonEntry = {
    address: "123 Main St",
    _id: "abc123",
    hack: {
        projectName: "Hackathon Project",
        problemStatement: "Solve this problem",
        solutionDescription: "Our solution involves...",
        implementationDescription: "We implemented this using...",
        technologyStack: ["Node.js", "React", "MongoDB"]
    },
    teamMembers: [
        { name: "John Doe", email: "john.doe@example.com", role: "Developer" },
        { name: "Jane Smith", email: "jane.smith@example.com", role: "Designer" }
    ],
    eval: [
        {
            coherenceScore: 4,
            feasibilityScore: 3,
            innovationScore: 5,
            funScore: 4,
            evaluationRemarks: "Great job!",
            codeSnippets: [
                { code: "const x = 5", comment: "Declare a variable", language: "JavaScript" }
            ]
        }
    ],
    progressUpdates: [
        {
            progress: "Implemented feature X",
            wins: "Fixed bug Y",
            losses: "Encountered issue Z",
            gamePlan: "Next steps...",
            actionItems: ["Fix bug A", "Implement feature B"],
            codeSnippets: [
                { code: "const y = 10", comment: "Declare another variable", language: "JavaScript" }
            ]
        }
    ]
};


---
# <u>User</u>

what did you just do?

---
# <u>Assistant</u>

I provided an example entry for a Hackathon, following the structure defined by the type `HackathonEntry`. This entry includes information such as the project address, ID, hackathon project attributes, team members, evaluation scores, and progress updates. This example entry showcases the use of the defined types and their corresponding properties to create a cohesive representation of a hackathon entry.

---
# <u>User</u>

