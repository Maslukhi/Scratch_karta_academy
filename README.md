# Scratch Stars Academy

Scratch programming education platform for students and teachers.

## Technologies used

-   **Frontend:** React + Vite + TypeScript + Tailwind CSS + shadcn/ui
-   **Backend:** Vercel Serverless Functions (TypeScript)
-   **AI:** Groq LLM (llama-3.3-70b) + Pinecone Vector Database

## Setting

```bash
# Setting dependencies
npm install

# Run development server
npm run dev
```

## Environment Configuration

Create file `.env` with the content:

```
GROQ_API_KEY=your_groq_api_key
PINECONE_API_KEY=your_pinecone_api_key
PINECONE_INDEX=scratch-academy
```

## Ingest data for Chatbot

```bash
npm run ingest
```

## Deploy go up Vercel

```bash
vercel --prod
```

## API Endpoints

| Method | Endpoint         | Describe                       |
| ------ | ---------------- | ------------------------       |
| GET    | `/api/products`  | Retrieve the product list|
| GET    | `/api/resources` | Retrieve the list of resources |
| POST   | `/api/messages`  | Send a contact message         |
| POST   | `/api/chat`      | Chat with AI Bot               |

## Directory Structure

```
├── api/                # Vercel Serverless Functions
│   ├── products.ts
│   ├── resources.ts
│   ├── messages.ts
│   ├── chat.ts
│   └── lib/
├── src/                # Frontend source
│   ├── components/
│   ├── pages/
│   ├── data/
│   └── assets/
├── public/
├── scripts/
│   └── ingest-data.ts
└── package.json
```

---

© 2026 Scratch Karta Academy
