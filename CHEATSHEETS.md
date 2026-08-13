# Cheatsheets — quick commands & code snippets

Next.js (create app)
- npx create-next-app@latest --ts
- Start dev: npm run dev
- Build: npm run build
- Export: npm run start

Simple Next.js API route (pages/api/hello.ts)
```ts
import type { NextApiRequest, NextApiResponse } from 'next';
export default function handler(req: NextApiRequest, res: NextApiResponse) {
  res.status(200).json({ message: 'Hello' });
}
