# Student JARVIS V4
V4 adds separate accounts and cloud data.

1. Create a Supabase project.
2. In Supabase SQL Editor, run `supabase-schema.sql`.
3. Supabase Project Settings -> API: copy Project URL and anon/public key.
4. Replace the two placeholders at the top of `public/app.js`.
5. Push the project to GitHub and deploy on Vercel.
6. In Vercel Environment Variables add `OPENAI_API_KEY` and `OPENAI_MODEL=gpt-5.6-luna`.
Never put the OpenAI secret key in GitHub or browser code.

Each signed-in user has a separate database row protected by Row Level Security. If email confirmation is enabled, users must confirm their email before login.