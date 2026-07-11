# Net-Sense Creative Framework

Use this reference before choosing sticker scenarios, writing a character bible, or approving a production pilot.

## First Principle

A sticker is not primarily an illustration. It is a low-friction social action that helps someone respond inside a real relationship.

Optimize for:

`sendability = context fit x emotional precision x persona fit x visual recognition x surprise / social risk`

Technical beauty cannot rescue a sticker with no clear sending moment. A current catchphrase cannot rescue a sticker that loses meaning when the trend expires.

## Creative Direction

Define the pack before designing individual stickers:

- `target_audience`: who will send it.
- `relationship_context`: friend, partner, family, colleague, customer, mixed public chat, or another concrete relationship.
- `conversation_register`: intimate, polite, restrained, absurd, sarcastic, self-deprecating, deadpan, or custom.
- `persona.core`: the character's stable identity in one sentence.
- `persona.worldview`: the recurring belief that explains its reactions.
- `persona.social_posture`: how it protects status or relationships, such as soft refusal, polite surrender, self-mockery, or shameless confidence.
- `persona.signature_reaction`: a recognizable reaction pattern that can recur without repeating the same pose.
- `persona.verbal_fingerprint`: 3-6 short phrases or sentence rhythms, not a list of temporary catchphrases.
- `persona.visual_hook`: one silhouette, prop, face mark, posture, or transformation readable at phone size.

Do not define a persona only as species plus adjectives such as "cute healing puppy." That describes rendering, not behavior.

## Scenario Model

Plan every sticker as a social situation:

- `trigger_utterance`: what another person says or what just happened before this sticker is sent.
- `surface_message`: what the sender appears to communicate.
- `hidden_emotion`: what the sender is actually feeling.
- `social_move`: the relationship action, such as acknowledge, soften refusal, ask for help, claim credit, retreat, tease, defuse, or end a conversation.
- `meme_mechanism`: the reason it is memorable: contrast, understatement, overreaction, status reversal, literalization, delayed collapse, committed denial, or another explicit mechanism.
- `visual_hook`: the first readable visual beat.
- `punchline_frame`: the still moment or motion beat worth remembering or screenshotting.
- `use_case`: a one-sentence example of when to send it.

Weak concept: `tired + nodding + text "可以"`.

Strong concept: after "今晚能再改一版吗," the character politely nods while its body slowly collapses flat; the surface message is agreement, the hidden emotion is total shutdown, and the mechanism is verbal restraint versus physical collapse.

## Pack Portfolio

Build a portfolio instead of a flat emotion checklist.

- `utility`: frequent conversational work such as acknowledge, thank, apologize, ask, refuse, wait, and end chat.
- `persona`: reactions that make the sender feel represented, such as pretending to be calm, claiming credit, social retreat, or self-mockery.
- `wildcard`: a small number of high-surprise concepts with a strong visual punchline.

Recommended starting mixes:

- 8-pack: 4 utility, 3 persona, 1 wildcard.
- 16-pack: 8 utility, 5 persona, 3 wildcard.
- 24-pack: 12 utility, 8 persona, 4 wildcard.

Adjust for the audience, but keep at least one persona item and one wildcard in albums. Do not let several stickers perform the same social move with only different words.

## Concept Tournament

Use cheap reasoning before expensive generation.

1. Generate at least three text-only concepts for two anchor scenarios: one high-frequency utility scenario and one persona/wildcard scenario.
2. Make each concept use a different meme mechanism or visual hook.
3. Score the concepts before generating images.
4. Generate visual pilots only for the strongest directions.
5. Lock character/style only after both a utility pilot and a persona/wildcard pilot work. One visually clean but generic pilot is not enough.

Store candidates in `concept_candidates` with stable ids. Record `selected_concept_id` and a concrete selection reason.

## Creative Score

Score each selected concept from 1-5:

- `context_fit`: a specific sending moment is immediately available.
- `emotional_precision`: the concept expresses more than a generic emotion label.
- `persona_fit`: it could plausibly belong only to this character.
- `visual_hook`: the idea reads in about half a second at phone size.
- `surprise`: there is contrast, escalation, reversal, or another memorable turn.
- `sendability`: a user can imagine sending it without explanation.
- `social_safety`: its tone fits the target relationship and is unlikely to feel accidentally hostile, oily, or awkward.

Weight `context_fit` and `sendability` twice. Maximum weighted score is 45. Production admission requires:

- weighted score at least 32;
- `context_fit >= 4`;
- `sendability >= 4`;
- `persona_fit >= 3`;
- `social_safety >= 3`.

Utility stickers may have modest surprise, but they still need a character-specific visual hook. Do not inflate scores to pass a favorite drawing; revise the concept instead.

## Trend Use

Net sense is not a pile of current slang. Treat trends as a volatile surface layer:

- Record `trend_signal`, `observed_at`, `source_context`, and `trend_ttl_days` when a concept depends on a trend.
- Preserve the underlying social situation so the sticker still works after the phrase cools down.
- Reject direct copies of existing meme artwork, copyrighted characters, celebrity likenesses, platform UI, or another sticker pack's signature composition.
- Prefer durable social tensions plus fresh wording or staging.

## Creative Failure Patterns

Reject or rewrite concepts when:

- the scenario can only be described as a generic emotion;
- the character could be replaced by any cute animal with no loss;
- the punchline is only the caption text;
- several stickers share the same social move, body pose, and timing;
- the concept needs an explanation before it becomes funny;
- the trend reference is the whole idea;
- the tone is unsafe for the intended relationship;
- the visual hook disappears at `240x240`;
- a clean technical pilot is used to lock a generic creative direction.

