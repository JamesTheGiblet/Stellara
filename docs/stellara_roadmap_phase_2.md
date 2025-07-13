🚀 Stellara Roadmap: Phase 2 - Engagement & Visual Polish (Months 4-7)

This document outlines the second phase of Stellara's development, focusing on expanding player interaction by introducing the "Influencer Mode" and enhancing the visual feedback to create a more engaging and aesthetically cohesive experience.
🎯 Phase Goal

To enable players to actively influence their civilization's evolution, provide compelling visual feedback that reflects philosophical and emotional states, and implement save/load functionality. This phase establishes both "Observer" and "Influencer" modes as distinct and engaging options.
🗓️ Timeline: Months 4-7
🚀 Tasks

1. Emotional Logic System Expansion (Month 4-5)

    1.1. Refine Existing Emotional Stats & Influence:

        Action: Deepen the impact of existing emotional_stats (Trust, Pride, Grief, Curiosity) on behavior_tree_modifiers and growth_factor_influences.

        Details: For example, high Pride might increase combat_aggression but decrease diplomacy_willingness. High Curiosity might boost exploration_speed and knowledge_gain. Implement more nuanced emotional thresholds for specific behaviors.

    1.2. Implement "Emotional Mutation":

        Action: Develop a system where significant events (e.g., catastrophic loss, major discovery) or prolonged philosophical states can trigger changes in emotional_stats.

        Details: A "Trauma Event" might significantly increase Grief, leading to a temporary decrease in Curiosity or Trust. A "Major Discovery" might boost Curiosity and Pride.

2. influencer_controls Development (Month 4-6)

    2.1. Nudge Philosophical Tones:

        Action: Create UI elements (e.g., sliders, buttons) that allow the player to subtly nudge their civilization's philosophy_archetype towards another (e.g., slightly increasing Empiricism's influence on a Symbiotist fleet).

        Details: These nudges should have a gradual, cumulative effect, not instant changes.

    2.2. Trigger Environmental Events:

        Action: Implement player-activated triggers for specific environmental_events (e.g., "Spawn Minor Anomaly", "Introduce Resource Fluctuation", "Initiate Hostile Encounter").

        Details: These events will feed into the event_orchestrator and trigger the simulation_loop responses.

    2.3. Inject Mutations or Override Traits:

        Action: Provide player tools to inject_mutations (e.g., force a fleet_trait like "increased shield strength") or temporarily override_behavior_tree_modifiers (e.g., force a "retreat" decision in combat).

        Details: These should have cooldowns or resource costs to prevent abuse and maintain challenge.

    2.4. Influence Emotional Stats:

        Action: Allow players to directly influence specific emotional_stats with a limited effect (e.g., "Boost Trust," "Reduce Grief").

        Details: This could be tied to a "player influence resource" that regenerates over time.

3. pixel_prompt_engine & ai_asset_forge (Basic) (Month 4-6)

    3.1. Develop Initial Prompt Templates:

        Action: Create a library of prompt_templates for generating basic pixel art assets (e.g., "Empiricist Cruiser: sleek, data-rich panels", "Entropyist Planet: chaotic, fractured surface").

        Details: These templates will be simple strings that can be used with a placeholder AI image generation API or a pre-generated sprite library for MVP.

    3.2. Integrate Basic AI Asset Generation Interface:

        Action: Implement a simple internal tool or script that can take a prompt_template and output a sprite_id or placeholder_image_url.

        Details: For MVP, this might just select from a pre-defined set of pixel art sprites that visually match the philosophical descriptions. The goal is to establish the pipeline for AI-driven assets.

4. event_feed_overlay & heatmap_visualizer (Month 5-7)

    4.1. Real-time Event Feed Development:

        Action: Build a dynamic UI overlay that displays real_time_consequences and lore_entries as they occur in the simulation.

        Details: This feed should be scrollable and timestamped, providing a narrative log of the civilization's journey.

    4.2. Basic Heatmap Visualizer Implementation:

        Action: Create a simple visual representation (e.g., a grid or simplified map) that can display ideological_spread (e.g., color-coding sectors by dominant philosophy) or resource_density across the simulated universe.

        Details: This will be an abstract, symbolic visualization, not a detailed map.

5. universe_loop (Basic Environmental Reactions) (Month 4-5)

    5.1. Implement Basic Environmental Reactions:

        Action: Expand the universe_loop to include simple environmental_responses to civilization growth_patterns or resource_consumption.

        Details: For example, rapid resource extraction might lead to resource_depletion_events in a sector, or prolonged combat might attract hostile_anomalies.

6. save_state_manager (Month 6-7)

    6.1. Implement Save & Load Functionality:

        Action: Develop the system to save the entire simulation state (philosophy, fleet stats, emotional logic, event history, environmental state) to a file or database.

        Details: Implement a corresponding load function to resume a previous simulation. For MVP, this can be a local file system save.

🧪 Tests

1. Influencer Mode Responsiveness Tests (Throughout Month 4-6)

    Scenario: Player uses each influencer_control tool.

    Check: Verify that player_interventions have observable and logical effects on the simulation (e.g., nudging philosophy actually shifts biases over time, triggering an event causes the expected simulation_loop response).

2. Visual Feedback Accuracy Tests (Month 5-7)

    Scenario: Observe the GUI elements and generated_assets during various simulation states.

    Check: Ensure visual_feedback (e.g., dashboard stats, event feed, heatmap) accurately reflects philosophical_states, emotional_changes, and environmental_conditions. Verify that generated pixel_art (even placeholders) aligns with philosophical themes.

3. Emotional System Dynamics Tests (Month 5)

    Scenario: Introduce specific events (positive/negative) and observe emotional_stat changes.

    Check: Test if emotions_evolve realistically based on defined triggers and influence behavior as designed. For example, does a "catastrophic loss" event lead to an increase in Grief and a corresponding change in fleet behavior?

4. Integration Tests (Month 7)

    Scenario: Run full simulations using both Observer and Influencer modes, including saving and loading.

    Check: Ensure all new modules (influencer_controls, event_feed_overlay, save_state_manager) integrate seamlessly with the core simulation_loop established in Phase 1 without introducing regressions or performance issues.

✅ Validity Tests

1. Meaningful Influence (Month 7)

    Question: Do player actions in Influencer Mode feel impactful and provide clear feedback, making the player feel like an active architect?

    Method: Internal playtesting and targeted user feedback. Are players able to achieve desired shifts in their civilization's trajectory through their interventions? Is the feedback loop clear enough for them to understand the consequences of their actions?

2. Aesthetic Cohesion (Month 7)

    Question: Do the minimalist pixel art and Tron-inspired GUI create a cohesive and appealing visual experience that enhances the philosophical theme?

    Method: Visual review and aesthetic critique. Does the art style effectively communicate the abstract concepts without being distracting? Does the UI feel intuitive and visually consistent?

3. Emergent Storytelling Quality (Month 7)

    Question: Do the event feed and early lore entries provide a compelling sense of evolving narrative and history for the civilization?

    Method: Review of generated event_feed logs and lore_entries. Do they tell a coherent and interesting story about the civilization's journey? Does the emotional feedback contribute to this narrative?

✨ MVP Point: Interactive Simulation

Upon successful completion of Phase 2, Stellara will achieve its second MVP:

    Players can now actively influence their civilization's evolution through influencer_controls, nudging philosophies, triggering events, and modifying traits.

    The simulation provides compelling visual feedback through a real_time_event_feed and a basic heatmap_visualizer, reflecting philosophical_states, emotional_changes, and environmental_conditions.

    The game features functional save and load capabilities, allowing players to resume their philosophical experiments.

    This phase fully establishes both the "Observer Mode" and "Influencer Mode" as distinct, engaging, and integrated options, providing a dynamic experience of passive observation and active shaping.
