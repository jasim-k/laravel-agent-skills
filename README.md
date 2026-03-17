# Claude Code Skills

A collection of Claude Code skills for Laravel, Vue 3, and full-stack web development.

Each skill is a structured set of rules and examples that guides Claude to follow best practices for a specific technology or pattern.

## Skills

| Skill | Description |
|-------|-------------|
| [laravel-inertia-vue](laravel-inertia-vue) | Laravel + Inertia.js + Vue 3 full-stack patterns |

## How to Use a Skill

Copy the skill directory into your project's `.claude/skills/` folder:

```bash
cp -r laravel-inertia-vue /path/to/your-project/.claude/skills/
```

Claude Code will automatically pick up the skill when working in that project.

---

### [laravel-inertia-vue](laravel-inertia-vue)

Laravel 12 + Inertia.js + Vue 3 full-stack patterns using the Vue 3 Composition API (`<script setup lang="ts">`).

**24 rules across 5 categories:**

| Category | Rules | Priority |
|----------|-------|----------|
| Page Components | 6 | CRITICAL |
| Forms & Validation | 8 | CRITICAL |
| Navigation | 5 | HIGH |
| Shared Data | 4 | HIGH |
| Layouts | 1 | CRITICAL |

**Covers:**
- Page component structure with `<script setup lang="ts">` and `defineProps<Props>()`
- Persistent layouts via `defineOptions({ layout: AppLayout })`
- Forms with `useForm` composable and `v-model` bindings
- Validation error display and ARIA accessibility
- File uploads with progress tracking
- Form dirty state and navigation blocking
- Navigation with `<Link>` and `router.*` methods
- Shared data (`auth`, `flash`, `ziggy`) via `usePage()`
- Named routes with Ziggy
- Partial reloads with `router.reload({ only: [] })`

**Example prompts:**
- `How do I share data from Laravel to a Vue 3 component with Inertia?`
- `Create an Inertia page with a form using useForm composable`
- `Set up a persistent layout in Vue 3 with Inertia`
- `Show me how to handle file uploads with progress in Inertia Vue`

## References

- [Inertia.js docs](https://inertiajs.com/)
- [Vue 3 docs](https://vuejs.org/)
- [Laravel docs](https://laravel.com/docs)
- [Claude Code skills guide](https://docs.anthropic.com/claude-code)
