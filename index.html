import React, { useState, useEffect, useRef } from 'react';

// Helper function to sort podcasts by editing stage
const sortPodcastsByStage = (podcasts) => {
  const stageOrder = { 'ready': 1, 'editing': 2, 'need': 3 };
  if (!Array.isArray(podcasts)) {
    console.error("sortPodcastsByStage received non-array input:", podcasts);
    return [];
  }
  return [...podcasts].sort((a, b) => {
    return stageOrder[a.editingStage] - stageOrder[b.editingStage];
  });
};

// Main App Component - now acts as the single page
const App = () => {
  // Mock Data for Podcasts, now with external links for clips
  // All data is defined within the App component for single-file consolidation
  const initialMockPodcasts = [
    // Ready to Post
    {
      id: 'podcast-intro-bolder',
      title: 'Intro to Bolder',
      description: 'An introductory episode to the Bolder Adventure Park.',
      editingStage: 'ready',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'intro-full', title: 'Full 1', url: 'https://drive.google.com/file/d/1odo_6qINzfSHP7AUmyZLk1ENLtOQjMr5/view?usp=drive_link', description: 'The complete introduction to Bolder Adventure Park.', transcript: 'This is the transcript for the Intro to Bolder full podcast. It covers the initial concept, challenges, and success of opening day. You can add more detailed content here.' }] },
        { type: 'long', label: 'Long Clips',
          clips: [
            { id: 'intro-long-1', title: 'Long 1', url: 'https://drive.google.com/file/d/1Y9p2YVK7OgKCEhUJKLCVgG3zAQiZ97J6/view?usp=drive_link', description: 'A longer video highlight from the Intro to Bolder podcast.' },
            { id: 'intro-long-2', title: 'Long 2', url: 'https://drive.google.com/file/d/12_NN4MaI-6AxYj2FEoDqra_BIYhE9HJL/view?usp=drive_link', description: 'Intro to Bolder Long Clip 2.' },
            { id: 'intro-long-3', title: 'Long 3', url: 'https://drive.google.com/file/d/1YdB9uI4J04qP_zbmZqtnt5o03cTxzPoy/view?usp=drive_link', description: 'Intro to Bolder Long Clip 3.' },
            { id: 'intro-long-4', title: 'Long 4', url: 'https://drive.google.com/file/d/1ScYKPnh_YdjSWtUadsRfw3W8hkdxh-ZS/view?usp=drive_link', description: 'Intro to Bolder Long Clip 4.' },
          ]
        },
        { type: 'short', label: 'Short Clips',
          clips: [
            { id: 'intro-short-1', title: 'Short 1', url: 'https://drive.google.com/file/d/1LQB0BdNobyYAuJhGx-qRfSbA1A75LdAp/view?usp=drive_link', description: 'Intro to Bolder Short Clip 1.' },
            { id: 'intro-short-2', title: 'Short 2', url: 'https://drive.google.com/file/d/1IgzJJbdu6J_NULBYj5nlRijE9PmwxMQi/view?usp=drive_link', description: 'Intro to Bolder Short Clip 2.' },
            { id: 'intro-short-3', title: 'Short 3', url: 'https://drive.google.com/file/d/13z6M4ueqpO96mvqufD2lWComy1WE-zdq/view?usp=drive_link', description: 'Intro to Bolder Short Clip 3.' },
            { id: 'intro-short-4', title: 'Short 4', url: 'https://drive.google.com/file/d/1-3h7F4T_ep97J2-A_w5znLFwRLNnR-gD/view?usp=drive_link', description: 'Intro to Bolder Short Clip 4.' },
            { id: 'intro-short-5', title: 'Short 5', url: 'https://drive.google.com/file/d/1pwLgmbX8rJphfbLoUstbsk4uXNpnyk0F/view?usp=drive_link', description: 'Intro to Bolder Short Clip 5.' },
            { id: 'intro-short-6', title: 'Short 6', url: 'https://drive.google.com/file/d/1TUvmoXFq0R8bjcvHdzqSHMrJ2jHZHDZb/view?usp=drive_link', description: 'Intro to Bolder Short Clip 6.' },
            { id: 'intro-short-7', title: 'Short 7', url: 'https://drive.google.com/file/d/1lxu71bkvCOIYp-gVWDD9kdTmPh6HyyK4/view?usp=drive_link', description: 'Intro to Bolder Short Clip 7.' },
            { id: 'intro-short-8', title: 'Short 8', url: 'https://drive.google.com/file/d/1klmEEXlCpezd5uKn6jdtpB_lGPvepUSe/view?usp=drive_link', description: 'Intro to Bolder Short Clip 8.' },
            { id: 'intro-short-9', title: 'Short 9', url: 'https://drive.google.com/file/d/19e7RtbS9idAptJDouYRm_r292cMtoZ-f/view?usp=drive_link', description: 'Intro to Bolder Short Clip 9.' },
            { id: 'intro-short-10', title: 'Short 10', url: 'https://drive.google.com/file/d/16Rec-Tim5De5GnPw1XUgfSRux9aEzlHV/view?usp=drive_link', description: 'Intro to Bolder Short Clip 10.' },
            { id: 'intro-short-11', title: 'Short 11', url: 'https://drive.google.com/file/d/1wmhNCbidgVDf0DHbus4_90XMjRk6OXsu/view?usp=drive_link', description: 'Intro to Bolder Short Clip 11.' },
            { id: 'intro-short-12', title: 'Short 12', url: 'https://drive.google.com/file/d/1teJi04RduFc2FzcF-ChzBnJwS32pwJ6C/view?usp=drive_link', description: 'Intro to Bolder Short Clip 12.' },
            { id: 'intro-short-13', title: 'Short 13', url: 'https://drive.google.com/file/d/13l_Bs_xK9tFdSc5NbURAFti_9XcAzs2N/view?usp=drive_link', description: 'Intro to Bolder Short Clip 13.' },
            { id: 'intro-short-14', title: 'Short 14', url: 'https://drive.google.com/file/d/1i1W78MNVo5LiIHv0xJOpfwZ1yj6c_xOC/view?usp=drive_link', description: 'Intro to Bolder Short Clip 14.' },
            { id: 'intro-short-15', title: 'Short 15', url: 'https://drive.google.com/file/d/1fLwpdJ1zINFIBiZIi84EG0jCiCbR3Cjs/view?usp=drive_link', description: 'Intro to Bolder Short Clip 15.' },
          ]
        }
      ]
    },
    {
      id: 'podcast-duke-paul',
      title: 'Duke and Paul',
      description: 'An engaging chat with Duke and Paul. All related video clips are organized here.',
      editingStage: 'ready',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'duke-full', title: 'Full 1', url: 'https://drive.google.com/file/d/1iGYqwOf3ugoksyjff49PnaVCOBpfDL3F/view?usp=drive_link', description: 'The full podcast episode with Duke and Paul.', transcript: 'This is the transcript for the full Duke and Paul podcast. It delves into their engaging conversation and insights.' }] },
        { type: 'long', label: 'Long Clips',
          clips: [
            { id: 'duke-long-1', title: 'Long 1', url: 'https://drive.google.com/file/d/1Itw87ZoZv4ENll15_bKuEjZoFh9G4cd-/view?usp=drive_link', description: 'Duke & Paul Long Clip 1.' },
            { id: 'duke-long-2', title: 'Long 2', url: 'https://drive.google.com/file/d/16JtOFjSRmoOwxe_T1ym8UCtR1K6eT4gU/view?usp=drive_link', description: 'Duke & Paul Long Clip 2.' },
            { id: 'duke-long-3', title: 'Long 3', url: 'https://drive.google.com/file/d/1oGSyn3KVr2Qg2N6tD6svQTG3ARg0oADo/view?usp=drive_link', description: 'Duke & Paul Long Clip 3.' },
            { id: 'duke-long-4', title: 'Long 4', url: 'https://drive.google.com/file/d/1wn8mHEpv26FLCNNHW79dEc5V_Wz1soYt/view?usp=drive_link', description: 'Duke & Paul Long Clip 4.' },
            { id: 'duke-long-5', title: 'Long 5', url: 'https://drive.google.com/file/d/1jiDw2xepGZYpnJRl8c7fWc3D_rnRptia/view?usp=drive_link', description: 'Duke & Paul Long Clip 5.' },
          ]
        },
        { type: 'short', label: 'Short Clips',
          clips: [
            { id: 'duke-short-1', title: 'Short 1', url: 'https://drive.google.com/file/d/19e-lhe8NcPnusOzFkOPzZXH3b2TpO9yA/view?usp=sharing', description: 'First short clip with Duke and Paul.', transcript: 'Transcript for Duke & Paul Short 1: This clip highlights a key opening statement.' },
            { id: 'duke-short-2', title: 'Short 2', url: 'https://drive.google.com/file/d/1g3Mj615Z5cW9Oa2vW70yEyGXGAdcJxvg/view?usp=sharing', description: 'Second short clip with Duke and Paul.', transcript: 'Transcript for Duke & Paul Short 2: Focuses on a specific point made during their discussion.' },
            { id: 'duke-short-3', title: 'Short 3', url: 'https://drive.google.com/file/d/188YTo8vU_98u1TdJwwZwYRzay8eehgZs/view?usp=sharing', description: 'Third short clip with Duke and Paul.', transcript: 'Transcript for Duke & Paul Short 3: A memorable quote or exchange.' },
            { id: 'duke-short-4', title: 'Short 4', url: 'https://drive.google.com/file/d/104EHkXUTuf_K_EnM7yUqcuLweotHl1Hu/view?usp=drive_link', description: 'Fifth short clip with Duke and Paul.', transcript: 'Transcript for Duke & Paul Short 4: Discusses a specific example.' },
            { id: 'duke-short-5', title: 'Short 5', url: 'https://drive.google.com/file/d/19oCDps3dl208tbOGXr7AvFB1V7kpUzqW/view?usp=sharing', description: 'Sixth short clip with Duke and Paul.', transcript: 'Transcript for Duke & Paul Short 5: A humorous or unexpected moment.' },
            { id: 'duke-short-6', title: 'Short 6', url: 'https://drive.google.com/file/d/1Sod-_Hr-6B0DHvrFPxrTodpub_qajf9T/view?usp=sharing', description: 'Seventh short clip with Duke and Paul.', transcript: 'Transcript for Duke & Paul Short 6: Concluding remarks or a call to action.' },
            { id: 'duke-short-7', title: 'Short 7', url: 'https://drive.google.com/file/d/1sRpit1zSwtdRsHQvFTZxLE3pY7-eEU4T/view?usp=drive_link', description: 'Duke & Paul Short Clip 7.' },
            { id: 'duke-short-8', title: 'Short 8', url: 'https://drive.google.com/file/d/1KSrtmJbfuUAH8ZhnaetxFgG2plRIti71/view?usp=drive_link', description: 'Duke & Paul Short Clip 8.' },
            { id: 'duke-short-9', title: 'Short 9', url: 'https://drive.google.com/file/d/17jQ2T4z6G019NUhZS8dLeaLZy_IdJTdE/view?usp=drive_link', description: 'Duke & Paul Short Clip 9.' },
            { id: 'duke-short-10', title: 'Short 10', url: 'https://drive.google.com/file/d/1kcL7BZMggB1dT8_HKrL0AhA919mg_AF5/view?usp=drive_link', description: 'Duke & Paul Short Clip 10.' },
          ]
        }
      ]
    },
    {
      id: 'podcast-raising-capital',
      title: 'Raising Capital',
      description: 'Strategies and insights on effectively raising capital.',
      editingStage: 'ready',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'capital-full', title: 'Full 1', url: 'https://drive.google.com/file/d/1slKXuwTkCZGdowOIciApq9ikdvR-nm0T/view?usp=drive_link', description: 'The complete episode on raising capital.', transcript: 'Transcript for Raising Capital full podcast: Covers all aspects of capital acquisition, from seed funding to IPOs.' }] },
        { type: 'long', label: 'Long Clips',
          clips: [
            { id: 'capital-long-1', title: 'Long 1', url: 'https://drive.google.com/file/d/1sg4F3tmkptmCm97RVzrm3mbw2rZlB18a/view?usp=drive_link', description: 'Raising Capital Long Clip 1.' },
            { id: 'capital-long-2', title: 'Long 2', url: 'https://drive.google.com/file/d/1vgQf6QffxK_Xx-8aLGYwv2DMaMF6rABJ/view?usp=drive_link', description: 'Raising Capital Long Clip 2.' },
            { id: 'capital-long-3', title: 'Long 3', url: 'https://drive.google.com/file/d/17JEWV4GcIbpH8f8M4drOKBXdicA-v7CU/view?usp=drive_link', description: 'Raising Capital Long Clip 3.' },
            { id: 'capital-long-4', title: 'Long 4', url: 'https://drive.google.com/file/d/1xW57Pvj0uGqagu4cYR02gjt9YOz3T6x-/view?usp=drive_link', description: 'Raising Capital Long Clip 4.' },
            { id: 'capital-long-5', title: 'Long 5', url: 'https://drive.google.com/file/d/1S4PfIN5gQXdhiDHtUsOvLB3npV74MkCq/view?usp=drive_link', description: 'Raising Capital Long Clip 5.' },
          ]
        },
        { type: 'short', label: 'Short Clips',
          clips: [
            { id: 'capital-short-1', title: 'Short 1', url: 'https://drive.google.com/file/d/138Vj_JcthcneSdOP7MGQsRjJrg9rU0Ec/view?usp=drive_link', description: 'Raising Capital Short Clip 1.' },
            { id: 'capital-short-2', title: 'Short 2', url: 'https://drive.google.com/file/d/1Z0o42AeJm0R_FJ8jQG3L3Zwm_pwwTdtW/view?usp=drive_link', description: 'Raising Capital Short Clip 2.' },
            { id: 'capital-short-3', title: 'Short 3', url: 'https://drive.google.com/file/d/1eMg8cMDnMbetG0wdGpq-bmvw7XCuQ752/view?usp=drive_link', description: 'Raising Capital Short Clip 3.' },
            { id: 'capital-short-4', title: 'Short 4', url: 'https://drive.google.com/file/d/13PnQ13hcK9BvHKbl5pskPZABvE9ocqUd/view?usp=drive_link', description: 'Raising Capital Short Clip 4.' },
            { id: 'capital-short-5', title: 'Short 5', url: 'https://drive.google.com/file/d/1o8vdsgU0wouxzWHUrmmxRob0kqaCugiy/view?usp=drive_link', description: 'Raising Capital Short Clip 5.' },
            { id: 'capital-short-6', title: 'Short 6', url: 'https://drive.google.com/file/d/1ade7rgeww6O4trDbU596DdnQWh0qUy_O/view?usp=drive_link', description: 'Raising Capital Short Clip 6.' },
            { id: 'capital-short-7', title: 'Short 7', url: 'https://drive.google.com/file/d/1DNyLuqnu6N719CSG1lX3VFLuMdVq-KHW/view?usp=drive_link', description: 'Raising Capital Short Clip 7.' },
            { id: 'capital-short-8', title: 'Short 8', url: 'https://drive.google.com/file/d/1DeKT-iUfk4ZlWq0tqrFVI6qo6OpmOI-b/view?usp=drive_link', description: 'Raising Capital Short Clip 8.' },
            { id: 'capital-short-9', title: 'Short 9', url: 'https://drive.google.com/file/d/1p2izTbN57ePfHzZHL7-PXC_C4U8gC4IZ/view?usp=drive_link', description: 'Raising Capital Short Clip 9.' },
            { id: 'capital-short-10', title: 'Short 10', url: 'https://drive.google.com/file/d/1Dn29nWAdWXGLnS690UWuu19VOSSink4e/view?usp=drive_link', description: 'Raising Capital Short Clip 10.' },
            { id: 'capital-short-11', title: 'Short 11', url: 'https://drive.google.com/file/d/16BByYcTpnYUgXoiDvjz2IhdB98vMGoEx/view?usp=drive_link', description: 'Raising Capital Short Clip 11.' },
            { id: 'capital-short-12', title: 'Short 12', url: 'https://drive.google.com/file/d/1S7K9XdfDiCEYslJDe3leJR9QQm4YvgMI/view?usp=drive_link', description: 'Raising Capital Short Clip 12.' },
            { id: 'capital-short-13', title: 'Short 13', url: 'https://drive.google.com/file/d/1xcgmnEYnvvbBezHKYXaUaHmybCsoEUoj/view?usp=drive_link', description: 'Raising Capital Short Clip 13.' },
            { id: 'capital-short-14', title: 'Short 14', url: 'https://drive.google.com/file/d/1zD8GHIypCmHUHFlxamN3jE6REfMg2M_j/view?usp=drive_link', description: 'Raising Capital Short Clip 14.' },
            { id: 'capital-short-15', title: 'Short 15', url: 'https://drive.google.com/file/d/1KMBMuaL5NtiXfxsHg4O1YYPqwCoDpyIu/view?usp=drive_link', description: 'Raising Capital Short Clip 15.' },
            { id: 'capital-short-16', title: 'Short 16', url: 'https://drive.google.com/file/d/1l2pfLydQY4_q_SVgM8voTsmYdL0qoM1e/view?usp=drive_link', description: 'Raising Capital Short Clip 16.' },
            { id: 'capital-short-17', title: 'Short 17', url: 'https://drive.google.com/file/d/1v7YkfEcEj1YbsGqa3_F30K9UJTfeR1X9/view?usp=drive_link', description: 'Raising Capital Short Clip 17.' },
            { id: 'capital-short-18', title: 'Short 18', url: 'https://drive.google.com/file/d/1wnxcDAh2nEjHLThnV--LrTtAeE9W0W5I/view?usp=drive_link', description: 'Raising Capital Short Clip 18.' },
            { id: 'capital-short-19', title: 'Short 19', url: 'https://drive.google.com/file/d/106nqTHGXhOLscCxFaa-yFngEUgK_1SVN/view?usp=drive_link', description: 'Raising Capital Short Clip 19.' },
            { id: 'capital-short-20', title: 'Short 20', url: 'https://drive.google.com/file/d/11qqqAymHgtnQeN-CltxeE6JIYxVHQ1mU/view?usp=drive_link', description: 'Raising Capital Short Clip 20.' },
          ]
        }
      ]
    },
    {
      id: 'podcast-phil-paul', // Moved to ready
      title: 'Phil & Paul',
      description: 'A compelling discussion featuring Phil and Paul.',
      editingStage: 'ready',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'pp-full', title: 'Full 1', url: 'https://drive.google.com/file/d/13E68U8t9jSTQ8s4s6w01ksFZW408w2aV/view?usp=drive_link', description: 'The complete Phil and Paul conversation.', transcript: 'Transcript for Phil & Paul full podcast: Comprehensive discussion on their shared experiences.' }] },
        { // All Phil & Paul long clips consolidated here
          type: 'long', label: 'Long Clips',
          clips: [
            { id: 'pp-long-1', title: 'Long 1', url: 'https://drive.google.com/file/d/1xB3Wn-fRec-NTML_MuSb82gXPqPjTd04/view?usp=drive_link', description: 'Phil & Paul Long Clip 1.' },
            { id: 'pp-long-2', title: 'Long 2', url: 'https://drive.google.com/file/d/10B-RfllaCrw5jXVaVZvMwbD-5US5LuCV/view?usp=drive_link', description: 'Phil & Paul Long Clip 2.' },
            { id: 'pp-long-3', title: 'Long 3', url: 'https://drive.google.com/file/d/1m0Iy137HjR7GCq6_u8801QOVCAYYXf9S/view?usp=drive_link', description: 'Phil & Paul Long Clip 3.' },
            { id: 'pp-long-4', title: 'Long 4', url: 'https://drive.google.com/file/d/1lkWkKSu6O_hUsPph6IS6sruGT7cJMPR6/view?usp=drive_link', description: 'Phil & Paul Long Clip 4.' },
            { id: 'pp-long-5', title: 'Long 5', url: 'https://drive.google.com/file/d/1Rtb4Qq2kLjMKcIhm21Dcfo5gmh96TZvi/view?usp=drive_link', description: 'Phil & Paul Long Clip 5.' },
            { id: 'pp-long-6', title: 'Long 6', url: 'https://drive.google.com/file/d/13RFJu5O_RjseXu3Alci71XU0KsEYoDJy/view?usp=drive_link', description: 'Phil & Paul Long Clip 6.' },
          ]
        },
        { type: 'short', label: 'Short Clips',
          clips: [
            { id: 'pp-short-1', title: 'Short 1', url: 'https://drive.google.com/file/d/10xLLSCZGM_Le-h9nhUrF3ISJ8SoRBgM/view?usp=drive_link', description: 'Phil & Paul Short Clip 1.' },
            { id: 'pp-short-2', title: 'Short 2', url: 'https://drive.google.com/file/d/1Rx4cQUkXakjkBsfGnuabv2HjwNxINFk8/view?usp=drive_link', description: 'Phil & Paul Short Clip 2.' },
            { id: 'pp-short-3', title: 'Short 3', url: 'https://drive.google.com/file/d/1OLFZtKqh5miS6DuZJrtY2b6m42_qcguQ/view?usp=drive_link', description: 'Phil & Paul Short Clip 3.' },
            { id: 'pp-short-4', title: 'Short 4', url: 'https://drive.google.com/file/d/1NtzlJEOVLZhIJelNHHz_ds-Ywi8W6awu/view?usp=drive_link', description: 'Phil & Paul Short Clip 4.' },
            { id: 'pp-short-5', title: 'Short 5', url: 'https://drive.google.com/file/d/1Zyd48qS2luWz0DVTf7VDQ62I0ovABAx6/view?usp=drive_link', description: 'Phil & Paul Short Clip 5.' },
            { id: 'pp-short-6', title: 'Short 6', url: 'https://drive.google.com/file/d/1BclCZKniKHIGWyGLn-PY-cSg5cyL4xkP/view?usp=drive_link', description: 'Phil & Paul Short Clip 6.' },
            { id: 'pp-short-7', title: 'Short 7', url: 'https://drive.google.com/file/d/1qHnALZglSCVziQfHZ-uz9VgpdnZIMkvg/view?usp=drive_link', description: 'Phil & Paul Short Clip 7.' },
            { id: 'pp-short-8', title: 'Short 8', url: 'https://drive.google.com/file/d/12O5ITt9PFpykWBUCDnJuLu7hZ36Xrew8/view?usp=drive_link', description: 'Phil & Paul Short Clip 8.' },
            { id: 'pp-short-9', title: 'Short 9', url: 'https://drive.google.com/file/d/1GbTeNlQ7E8z4ghAdxWhCSMoOoPp5BvPm/view?usp=drive_link', description: 'Phil & Paul Short Clip 9.' },
            { id: 'pp-short-10', title: 'Short 10', url: 'https://drive.google.com/file/d/1RJaxkRgDLon7rGI3nPj0JJz0Fh6XBooW/view?usp=drive_link', description: 'Phil & Paul Short Clip 10.' },
            { id: 'pp-short-11', title: 'Short 11', url: 'https://drive.google.com/file/d/1SP0RpWurBAJqMxU3eeIxS-Cnpu9cXsa3/view?usp=drive_link', description: 'Phil & Paul Short Clip 11.' },
            { id: 'pp-short-12', title: 'Short 12', url: 'https://drive.google.com/file/d/1cDZtrriomJO0w0gqI9A0tJ1Acx2U_lll/view?usp=drive_link', description: 'Phil & Paul Short Clip 12.' },
            { id: 'pp-short-13', title: 'Short 13', url: 'https://drive.google.com/file/d/1dzU4VyERLo4_u1BfwU3_wqRj5_xPuha8/view?usp=drive_link', description: 'Phil & Paul Short Clip 13.' },
            { id: 'pp-short-14', title: 'Short 14', url: 'https://drive.google.com/file/d/1gdPvwhXToxlLBOVBE9WxTspWwjV4kFo6/view?usp=drive_link', description: 'Phil & Paul Short Clip 14.' },
            { id: 'pp-short-15', title: 'Short 15', url: 'https://drive.google.com/file/d/1Du9I8YHf1TDMUky8Ux2Z5jW3KroCeXHv/view?usp=drive_link', description: 'Phil & Paul Short Clip 15.' },
            { id: 'pp-short-16', title: 'Short 16', url: 'https://drive.google.com/file/d/1jra-RrSinSe_grC6u3uLHjE8adzFs7Ls/view?usp=drive_link', description: 'Phil & Paul Short Clip 16.' },
            { id: 'pp-short-17', title: 'Short 17', url: 'https://drive.google.com/file/d/1aJtMypGJi6cQXg_03juyjh_2sI4jsOaa/view?usp=drive_link', description: 'Phil & Paul Short Clip 17.' },
            { id: 'pp-short-18', title: 'Short 18', url: 'https://drive.google.com/file/d/1-KcIeX5U6WahoTz4_W8tF8Usx8Q9iGi3/view?usp=drive_link', description: 'Phil & Paul Short Clip 18.' },
            { id: 'pp-short-19', title: 'Short 19', url: 'https://drive.google.com/file/d/1aR7smhwT-CUdXZMy6NrhHE4O_vYnnsX1/view?usp=drive_link', description: 'Phil & Paul Short Clip 19.' },
            { id: 'pp-short-20', title: 'Short 20', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Phil & Paul Short Clip 20 (Placeholder).' },
          ]
        }
      ]
    },

    // In Editing
    {
      id: 'podcast-todd-jankins-paul',
      title: 'Todd Jankins & Paul',
      description: 'A compelling discussion featuring Todd Jankins and Paul.',
      editingStage: 'editing',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'tjp-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'The complete Todd Jankins and Paul episode.', transcript: 'Transcript for Todd Jankins & Paul full podcast: Detailed discussion on their collaborative projects.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'tjp-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Extended segment from Todd Jankins and Paul\'s discussion.', transcript: 'Transcript for Todd Jankins & Paul long clip: Extended segment on a specific industry trend.' }] },
        { type: 'short', label: 'Short Clips', clips: [{ id: 'tjp-short', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Top insights from Todd Jankins and Paul.', transcript: 'Transcript for Todd Jankins & Paul short clip: Key insights and actionable advice.' }] }
      ]
    },
    {
      id: 'podcast-todd-jankins-paul-2',
      title: 'Todd Jankins & Paul Part 2',
      description: 'The continuation of the engaging conversation with Todd Jankins and Paul.',
      editingStage: 'editing',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'tjp2-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Part 2 of the complete Todd Jankins and Paul episode.', transcript: 'Transcript for Todd Jankins & Paul Part 2 full podcast: Continuation of their in-depth conversation.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'tjp2-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Extended segment from Todd Jankins and Paul\'s Part 2 discussion.', transcript: 'Transcript for Todd Jankins & Paul Part 2 long clip: Focus on future predictions and industry shifts.' }] },
        { type: 'short', label: 'Short Clips', clips: [{ id: 'tjp2-short', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Highlights from Part 2 of Todd Jankins and Paul.', transcript: 'Transcript for Todd Jankins & Paul Part 2 short clip: Quick highlights from the second part.' }] }
      ]
    },

    // Need Editing
    {
      id: 'podcast-roller-coaster-build', // Moved to need editing
      title: 'Behind the Scenes: Roller Coaster Build',
      description: 'A comprehensive look at the construction of our most thrilling roller coaster, "The Gravity Gauntlet." Witness the engineering and dedication involved.',
      editingStage: 'need',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'rc-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'The full documentary on roller coaster construction.', transcript: 'Transcript for Roller Coaster Build full documentary: Details the entire construction process from design to completion.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'rc-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Extended time-lapse of the roller coaster build.', transcript: 'Transcript for Roller Coaster Build long clip: Shows the time-lapse with commentary on key construction phases.' }] },
        { type: 'short', label: 'Short Clips',
          clips: [
            { id: 'rc-short-1', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Short clip of track assembly.', transcript: 'Transcript for Roller Coaster Build Short 1: Focus on track assembly.' },
            { id: 'rc-short-2', title: 'Short 2', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Short 2', transcript: 'Transcript for Roller Coaster Build Short 2: Reactions during the first test run.' },
            { id: 'rc-short-3', title: 'Short 3', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Short 3', transcript: 'Transcript for Roller Coaster Build Short 3: Highlights of safety inspections.' },
          ]
        }
      ]
    },
    {
      id: 'podcast-park-opening', // Moved to need editing
      title: 'Park Opening Day Excitement',
      description: 'Relive the energy and excitement of Bolder Adventure Park\'s grand opening! Interviews with guests, staff, and a look at the inaugural ceremonies.',
      editingStage: 'need',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'po-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Full video of the park opening ceremony.', transcript: 'Transcript for Park Opening full video: The complete opening ceremony and speeches.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'po-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Extended interviews from opening day.', transcript: 'Transcript for Park Opening long clip: Extended interviews with first visitors and park staff.' }] },
        { type: 'short', label: 'Short Clips',
          clips: [
            { id: 'po-short-1', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Short clip of queue line antics.', transcript: 'Transcript for Park Opening Short 1: Fun moments from the queue line.' },
            { id: 'po-short-2', title: 'Short 2', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', description: 'Short 2', transcript: 'Transcript for Park Opening Short 2: The official ribbon cutting ceremony.' },
          ]
        }
      ]
    },
    {
      id: 'podcast-alex-paul',
      title: 'Alex & Paul',
      description: 'A deep dive into discussions with Alex and Paul on various topics.',
      editingStage: 'need',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'ap-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'The complete conversation with Alex and Paul.', transcript: 'Transcript for Alex & Paul full podcast: In-depth discussion on their collaborative work.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'ap-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'An extended video segment from Alex and Paul\'s discussion.', transcript: 'Transcript for Alex & Paul long clip: Extended segment on a challenging project.' }] },
        { type: 'short', label: 'Short Clips', clips: [{ id: 'ap-short', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Key takeaways and highlights from Alex and Paul.', transcript: 'Transcript for Alex & Paul short clip: Quick highlights and key insights.' }] }
      ]
    },
    {
      id: 'podcast-consulting',
      title: 'Consulting',
      description: 'Insights and advice on the world of consulting.',
      editingStage: 'need',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'consult-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Full episode on consulting strategies.', transcript: 'Transcript for Consulting full podcast: Comprehensive guide to consulting best practices.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'consult-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Detailed segment on specific consulting challenges.', transcript: 'Transcript for Consulting long clip: Detailed case study on a specific consulting challenge.' }] },
        { type: 'short', label: 'Short Clips', clips: [{ id: 'consult-short', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Quick tips for aspiring consultants.', transcript: 'Transcript for Consulting short clip: Actionable tips for new consultants.' }] }
      ]
    },
    {
      id: 'podcast-ryan-paul',
      title: 'Ryan DeJoy & Paul',
      description: 'Ryan DeJoy joins Paul for an exciting conversation.',
      editingStage: 'need',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'rdp-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Full episode with Ryan DeJoy and Paul.', transcript: 'Transcript for Ryan DeJoy & Paul full podcast: Their complete discussion on technology and innovation.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'rdp-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Extended discussion with Ryan DeJoy and Paul.', transcript: 'Transcript for Ryan DeJoy & Paul long clip: Extended segment on AI ethics.' }] },
        { type: 'short', label: 'Short Clips', clips: [{ id: 'rdp-short', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Highlights from Ryan DeJoy and Paul\'s talk.', transcript: 'Transcript for Ryan DeJoy & Paul short clip: Key moments from their tech discussion.' }] }
      ]
    },
    {
      id: 'podcast-paul-ethan',
      title: 'Paul Talking about Ethan',
      description: 'Paul shares his thoughts and stories about Ethan.',
      editingStage: 'need',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'pe-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'The complete podcast of Paul talking about Ethan.', transcript: 'Transcript for Paul Talking about Ethan full podcast: All of Paul\'s stories and reflections on Ethan.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'pe-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'An extended segment of Paul\'s stories about Ethan.', transcript: 'Transcript for Paul Talking about Ethan long clip: An extended personal anecdote.' }] },
        { type: 'short', label: 'Short Clips', clips: [{ id: 'pe-short', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Short, memorable moments of Paul discussing Ethan.', transcript: 'Transcript for Paul Talking about Ethan short clip: A particularly funny or touching moment.' }] }
      ]
    },
    {
      id: 'podcast-book-reviews',
      title: 'Book reviews x4',
      description: 'Four insightful book reviews in one episode.',
      editingStage: 'need',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'br-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'All four book reviews in detail.', transcript: 'Transcript for Book reviews x4 full podcast: Detailed analysis of four different books.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'br-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Extended discussions on selected book reviews.', transcript: 'Transcript for Book reviews x4 long clip: Extended discussion on the most impactful review.' }] },
        { type: 'short', label: 'Short Clips', clips: [{ id: 'br-short', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Quick summaries of each book review.', transcript: 'Transcript for Book reviews x4 short clip: Quick summaries of all four books.' }] }
      ]
    },
    {
      id: 'podcast-paul-pratham',
      title: 'Paul & Pratham',
      description: 'A joint discussion with Paul and Pratham.',
      editingStage: 'need',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'ppr-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'The complete Paul and Pratham episode.', transcript: 'Transcript for Paul & Pratham full podcast: Their complete joint discussion.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'ppr-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Extended discussion with Paul and Pratham.', transcript: 'Transcript for Paul & Pratham long clip: Extended segment on their collaborative project.' }] },
        { type: 'short', label: 'Short Clips', clips: [{ id: 'ppr-short', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Key insights from Paul and Pratham.', transcript: 'Transcript for Paul & Pratham short clip: Key insights and shared ideas.' }] }
      ]
    },
    {
      id: 'podcast-paul-gustavo',
      title: 'Paul & Gustavo',
      description: 'An insightful conversation between Paul and Gustavo.',
      editingStage: 'need',
      versions: [
        { type: 'full', label: 'Full Podcast', clips: [{ id: 'pg-full', title: 'Full 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'The complete Paul and Gustavo discussion.', transcript: 'Transcript for Paul & Gustavo full podcast: Their complete insightful conversation.' }] },
        { type: 'long', label: 'Long Clips', clips: [{ id: 'pg-long', title: 'Long 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Extended segment from Paul and Gustavo\'s conversation.', transcript: 'Transcript for Paul & Gustavo long clip: Extended segment on a philosophical topic.' }] },
        { type: 'short', label: 'Short Clips', clips: [{ id: 'pg-short', title: 'Short 1', url: 'https://www.learningcontainer.com/wp-content/uploads/2020/05/sample-mp4-file.mp4', mediaType: 'video', description: 'Memorable moments from Paul and Gustavo.', transcript: 'Transcript for Paul & Gustavo short clip: Memorable quotes and key points.' }] }
      ]
    },
  ];

  // State for podcasts in the Full Podcasts section (for drag and drop)
  const [podcasts, setPodcasts] = useState(() => sortPodcastsByStage(initialMockPodcasts));

  // States for managing dropdowns and selected tabs/clips within the single page
  const [openPodcastId, setOpenPodcastId] = useState(null); // Which podcast dropdown is open
  const [selectedVersionType, setSelectedVersionType] = useState({}); // Which version tab is selected for each podcast
  const [selectedClipId, setSelectedClipId] = useState({}); // Which specific clip is selected within a version tab
  const [showTranscript, setShowTranscript] = useState({}); // State to manage transcript visibility for each clip

  const dragItem = useRef(null);
  const dragOverItem = useRef(null);

  const handleDragStart = (e, index) => {
    dragItem.current = index;
    e.target.classList.add('opacity-50', 'border-2', 'border-indigo-500');
  };

  const handleDragEnter = (e, index) => {
    dragOverItem.current = index;
    e.target.classList.add('bg-indigo-50');
  };

  const handleDragOver = (e) => {
    e.preventDefault();
  };

  const handleDragLeave = (e) => {
    e.target.classList.remove('bg-indigo-50');
  };

  const handleDrop = (e) => {
    e.preventDefault();
    const draggedIndex = dragItem.current;
    const droppedIndex = dragOverItem.current;

    if (e.target && e.target.classList) {
        e.target.classList.remove('bg-indigo-50');
    }

    if (draggedIndex !== null && droppedIndex !== null && draggedIndex !== droppedIndex) {
      const newPodcasts = [...podcasts];
      const [draggedPodcast] = newPodcasts.splice(draggedIndex, 1);
      newPodcasts.splice(droppedIndex, 0, draggedPodcast);
      setPodcasts(newPodcasts);
    }

    dragItem.current = null;
    dragOverItem.current = null;
    if (e.target && e.target.classList) {
      e.target.classList.remove('opacity-50', 'border-2', 'border-indigo-500');
    }
  };

  const handleDragEnd = (e) => {
    if (e.target && e.target.classList) {
      e.target.classList.remove('opacity-50', 'border-2', 'border-indigo-500');
    }
    const allListItems = document.querySelectorAll('.podcast-list-item'); // Use a specific class for clarity
    allListItems.forEach(item => item.classList.remove('bg-indigo-50'));
  };

  // Helper for getting stage display
  const getStageDisplay = (stage) => {
    switch (stage) {
      case 'ready': return { text: 'Ready to Post', color: 'text-green-600', bg: 'bg-green-100' };
      case 'editing': return { text: 'In Editing', color: 'text-yellow-600', bg: 'bg-yellow-100' };
      case 'need': return { text: 'Need Editing', color: 'text-red-600', bg: 'bg-red-100' };
      default: return { text: 'Unknown Stage', color: 'text-gray-600', bg: 'bg-gray-100' };
    }
  };

  // Render the consolidated home page
  return (
    <div className="min-h-screen bg-gray-100 font-inter antialiased flex flex-col">
      <header className="bg-white shadow-md py-4">
        <div className="container mx-auto px-4 flex justify-center items-center">
          {/* Brand title acts as Home anchor */}
          <a href="#" onClick={() => window.scrollTo({ top: 0, behavior: 'smooth' })} className="text-3xl font-bold text-indigo-600 rounded-lg p-2 hover:bg-indigo-50 transition duration-300">
            BOLDER PODCASTS
          </a>
        </div>
      </header>

      <main className="flex-grow container mx-auto px-4 py-8">
        {/* PODCAST Section */}
        <section id="podcasts" className="mb-12 bg-white p-6 rounded-xl shadow-lg">
          <h2 className="text-4xl font-extrabold text-indigo-700 mb-8 text-center">PODCASTS</h2>
          <p className="text-gray-600 mb-6 text-center">Click a podcast title to expand details and access its versions. Drag and drop to reorder.</p>

          {/* Iterate over predefined stage order */}
          {['ready', 'editing', 'need'].map(stageKey => {
            const stagePodcasts = podcasts.filter(p => p.editingStage === stageKey);
            if (stagePodcasts.length === 0) return null;
            const stageInfo = getStageDisplay(stageKey);
            return (
              <div key={stageKey} className="mb-8">
                <h3 className="text-2xl font-bold mb-4 px-4 py-2 rounded-lg shadow-sm" style={{ color: stageInfo.color, backgroundColor: stageInfo.bg }}>
                  {stageInfo.text}
                </h3>
                <ul className="space-y-4">
                  {stagePodcasts.map((podcast, index) => {
                    const actualIndex = podcasts.findIndex(p => p.id === podcast.id);
                    const isOpen = openPodcastId === podcast.id;
                    // State for the currently selected version tab within this podcast item
                    const currentSelectedVersionType = selectedVersionType[podcast.id] || (podcast.versions.length > 0 ? podcast.versions[0].type : null);
                    // State for the currently selected clip within the active version tab
                    const currentSelectedClipId = selectedClipId[podcast.id] || null;

                    const currentVersion = podcast.versions.find(v => v.type === currentSelectedVersionType);
                    const currentClip = currentVersion?.clips?.find(c => c.id === currentSelectedClipId) || currentVersion?.clips?.[0]; // Default to first clip if none selected

                    return (
                      <li
                        key={podcast.id}
                        draggable="true"
                        onDragStart={(e) => handleDragStart(e, actualIndex)}
                        onDragEnter={(e) => handleDragEnter(e, actualIndex)}
                        onDragLeave={handleDragLeave}
                        onDragOver={handleDragOver}
                        onDrop={handleDrop}
                        onDragEnd={handleDragEnd}
                        className="podcast-list-item bg-gray-50 p-6 rounded-lg shadow-md hover:shadow-xl transition duration-300 ease-in-out cursor-grab active:cursor-grabbing group"
                      >
                        <div
                          className="flex justify-between items-center cursor-pointer"
                          onClick={() => {
                            setOpenPodcastId(openPodcastId === podcast.id ? null : podcast.id);
                            // Reset selected version/clip when opening a new podcast or closing
                            if (openPodcastId !== podcast.id) {
                              setSelectedVersionType(prev => ({ ...prev, [podcast.id]: podcast.versions[0]?.type }));
                              setSelectedClipId(prev => ({ ...prev, [podcast.id]: podcast.versions[0]?.clips?.[0]?.id }));
                              setShowTranscript(prev => ({ ...prev, [podcast.id]: false })); // Hide transcript when closing/reopening
                            }
                          }}
                        >
                          <h4 className="text-xl font-semibold text-gray-800 group-hover:text-indigo-600 transition duration-300">
                            {podcast.title}
                            <span className="ml-2 text-sm font-normal text-gray-500">({stageInfo.text})</span>
                          </h4>
                          <svg
                            className={`w-6 h-6 transform transition-transform duration-300 ${isOpen ? 'rotate-180' : ''}`}
                            fill="none"
                            stroke="currentColor"
                            viewBox="0 0 24 24"
                            xmlns="http://www.w3.org/2000/svg"
                          >
                            <path strokeLinecap="round" strokeLinejoin="round" strokeWidth="2" d="M19 9l-7 7-7-7"></path>
                          </svg>
                        </div>

                        {isOpen && (
                          <div className="mt-4 pt-4 border-t border-gray-200">
                            <p className="text-gray-600 mb-4">{podcast.description}</p>

                            {/* Version Tabs (Full Podcast, Long Clips, Short Clips) */}
                            {podcast.versions.length > 0 && ( // Ensure there are versions to display buttons
                                <div className="flex justify-center space-x-2 sm:space-x-4 mb-8 flex-wrap gap-y-2">
                                    {podcast.versions.map(version => (
                                        <button
                                            key={version.type}
                                            onClick={(e) => {
                                                e.stopPropagation(); // Prevent closing dropdown
                                                setSelectedVersionType(prev => ({ ...prev, [podcast.id]: version.type }));
                                                setSelectedClipId(prev => ({ ...prev, [podcast.id]: version.clips?.[0]?.id })); // Auto-select first clip of new tab
                                                setShowTranscript(prev => ({ ...prev, [podcast.id]: false })); // Hide transcript on tab change
                                            }}
                                            className={`
                                                px-3 py-1 sm:px-4 sm:py-2 rounded-full text-xs sm:text-sm font-semibold transition duration-300
                                                ${currentSelectedVersionType === version.type
                                                    ? 'bg-indigo-600 text-white shadow-md'
                                                    : 'bg-gray-200 text-gray-700 hover:bg-gray-300'
                                                }
                                            `}
                                        >
                                            {version.label}
                                        </button>
                                    ))}
                                </div>
                            )}

                            {/* Clip Titles within the selected Version Tab */}
                            {currentVersion && currentVersion.clips && currentVersion.clips.length > 0 ? (
                                <div className="mb-8">
                                    <h5 className="text-lg font-semibold text-gray-800 mb-4 text-center">Select a Clip:</h5>
                                    <div className="flex flex-wrap gap-2 justify-center mb-6">
                                        {currentVersion.clips.map(clip => (
                                            <button
                                                key={clip.id}
                                                onClick={(e) => {
                                                    e.stopPropagation();
                                                    // Open the Google Drive link in a new tab
                                                    window.open(clip.url, '_blank');
                                                }}
                                                className={`
                                                    px-3 py-1 rounded-full text-sm font-medium transition duration-300
                                                    bg-blue-100 text-blue-800 hover:bg-blue-200
                                                `}
                                            >
                                                {clip.title}
                                            </button>
                                        ))}
                                    </div>

                                    <p className="text-gray-600 text-center py-4">Click a clip title above to open the video in a new tab.</p>
                                </div>
                            ) : (
                                <p className="text-gray-600 text-center py-4">No clips available for this version.</p>
                            )}
                          </div>
                        )}
                      </li>
                    );
                  })}
                </ul>
              </div>
            );
          })}
        </section>
      </main>

      <footer className="bg-gray-800 text-gray-300 py-8 px-4 mt-auto">
        <div className="container mx-auto text-center md:flex md:justify-between md:items-center">
          <p className="mb-4 md:mb-0">&copy; 2025 Bolder Adventure Park Podcast. All rights reserved.</p>
          <div className="flex justify-center space-x-6">
            <a href="#" className="hover:text-white transition duration-300 rounded-lg p-2 hover:bg-gray-700">Privacy Policy</a>
            <a href="#" className="hover:text-white transition duration-300 rounded-lg p-2 hover:bg-gray-700">Terms of Service</a>
          </div>
        </div>
      </footer>
    </div>
  );
};

export default App;
