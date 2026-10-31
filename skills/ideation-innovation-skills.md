# Ideation & Innovation Skills

Four reusable agent-skill references for generating less predictable ideas, escaping familiar solution patterns, and exploring new research directions.

These are catalogued as upstream references, consistent with the Armory's reference-library approach. The skill implementations remain in their original repositories; follow each upstream repository's installation instructions and license when using or installing them.

## Creative Thinking for Research — Orchestra Research

- Skill: `creative-thinking-for-research`
- Source: https://github.com/Jensen-Yao/agents-skills/tree/main/skills/creative-thinking-for-research
- Direct instructions: https://github.com/Jensen-Yao/agents-skills/blob/main/skills/creative-thinking-for-research/SKILL.md
- License: MIT
- Purpose: Applies cognitive-science-informed creativity frameworks to research ideation, including bisociation/combinatorial creativity, problem reformulation, analogical transfer, constraint manipulation, inversion, abstraction, boundary exploration, and contradiction-based thinking.
- Best use: When an AI keeps circling familiar approaches or needs to explore non-obvious research directions across disciplines.

## Brainstorming Research Ideas — Orchestra Research

- Skill: `brainstorming-research-ideas`
- Source: https://github.com/Jensen-Yao/agents-skills/tree/main/skills/brainstorming-research-ideas
- Direct instructions: https://github.com/Jensen-Yao/agents-skills/blob/main/skills/brainstorming-research-ideas/SKILL.md
- License: MIT
- Purpose: Uses structured ideation lenses to move from vague curiosity to concrete research directions, including problem-first/solution-first thinking, abstraction shifts, contradiction hunting, and opportunity discovery.
- Best use: Starting a research direction, pivoting a project, or searching a field for underexplored questions.

## Generating Novel Ideas — Tristan Manchester

- Skill: `generating-novel-ideas`
- Source: https://github.com/tristanmanchester/agent-skills/tree/main/generating-novel-ideas
- Direct instructions: https://github.com/tristanmanchester/agent-skills/blob/main/generating-novel-ideas/SKILL.md
- Version observed: 2.1.0
- Purpose: General-purpose ideation for products, businesses, research, campaigns, and process changes. Uses distinct search directions, analogy transfer, contradiction solving, diversity checks, critique-and-repair, and practical tests.
- Best use: Generating differentiated product or project opportunities instead of producing a list of near-identical variations.
- Note: The upstream instructions explicitly caution against claiming originality without an appropriately scoped search.

## Brainstorming — jwynia

- Skill: `brainstorming`
- Source: https://github.com/jwynia/agent-skills/tree/main/skills/general/ideation/brainstorming
- Direct instructions: https://github.com/jwynia/agent-skills/blob/main/skills/general/ideation/brainstorming/SKILL.md
- License: MIT (declared in the skill)
- Purpose: Helps an agent expand a seed idea or escape convergent thinking. It makes obvious defaults explicit, separates the desired function from the assumed solution form, varies key axes, and imports mechanisms from unrelated domains.
- Best use: When brainstorming keeps returning the same predictable ideas, or when an early concept needs to be expanded in genuinely different directions.
- Supporting asset: The skill includes a constraint-entropy helper script in its upstream directory.

## Recommended sequence

1. **Brainstorming** — expose defaults and break out of the obvious solution cluster.
2. **Creative Thinking for Research** — use cross-domain and problem-reframing frameworks to create more unusual directions.
3. **Generating Novel Ideas** — develop a diverse portfolio of concrete, differentiated concepts.
4. **Brainstorming Research Ideas** — use the research-specific lenses when the opportunity is a scientific or technical research direction.
5. **External validation** — search relevant repositories, papers, products, patents, and current projects before describing any finalist as potentially unexplored.

## Important limitation

No ideation skill can prove that nobody has ever developed an idea. These skills improve the search process and reduce generic repetition; novelty still requires scoped external research. A lack of search results is evidence of an unobserved match, not proof of absolute originality.

## Armory usage rule

Treat these as complementary thinking tools, not a mandatory chain. Select the smallest useful combination for the task. Do not claim that multiple internal passes are independent agents unless they actually ran in isolated contexts.
