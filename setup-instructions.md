# Cresta SaaS Setup Instructions

## Prerequisites
- Node.js 18+ installed
- npm or yarn package manager

## Setup Steps

1. **Navigate to project directory**
   \`\`\`bash
   cd "cresta-saas (1)"
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   npm install
   # or
   yarn install
   \`\`\`

3. **Create environment file**
   \`\`\`bash
   cp .env.example .env.local
   # or create .env.local manually
   \`\`\`

4. **Add your API keys to .env.local**
   \`\`\`env
   GEMINI_API_KEY_1=your_first_gemini_api_key_here
   GEMINI_API_KEY_2=your_second_gemini_api_key_here
   \`\`\`

5. **Run the development server**
   \`\`\`bash
   npm run dev
   # or
   yarn dev
   \`\`\`

6. **Open in browser**
   Navigate to http://localhost:3000

## Troubleshooting

If you encounter build errors:
1. Delete node_modules and package-lock.json
2. Run `npm install` again
3. Make sure all dependencies are properly installed

## Getting Gemini API Keys

1. Go to https://makersuite.google.com/app/apikey
2. Create a new API key
3. Copy the key to your .env.local file
4. You can use the same key for both GEMINI_API_KEY_1 and GEMINI_API_KEY_2, or create two separate keys for better quota management
