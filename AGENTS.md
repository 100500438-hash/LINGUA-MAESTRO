<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

- AI content is generated via authenticated server functions in `src/lib/ai/learning.functions.ts` using strict zod schemas in `src/lib/ai/schemas.ts` — keeps prompts/keys server-side and output shape guaranteed.
- Per-language accent color comes from a `data-lang` attribute switching the `--lang` token — one component set themes both languages.
- Progress (levels, activity log) is read/written from the browser under RLS in `src/lib/progress.ts` — no server hop needed for user-owned rows.
