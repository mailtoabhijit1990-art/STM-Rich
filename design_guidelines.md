# Sleep Tracking Game - Design Guidelines

## Design Approach

**Selected Approach:** Reference-Based with Gaming Elements

Drawing inspiration from successful wellness and sleep tracking apps (Pokémon Sleep, Sleep Cycle, Headspace) combined with mobile game patterns. This sleep tracking game prioritizes engagement through gamification while maintaining a calming, restful aesthetic.

**Key Design Principles:**
- Calming and soothing visual language appropriate for sleep/wellness context
- Game mechanics that reward consistency without creating stress
- Clear data visualization that makes sleep patterns instantly understandable
- Minimal cognitive load for logging sleep (should be effortless)

## Typography

**Font Stack:** Poppins (primary), SF Pro Display (iOS fallback), Roboto (Android fallback)

**Hierarchy:**
- **Game Title/Headers:** Bold, 32-36pt
- **Screen Titles:** SemiBold, 24-28pt
- **Stats/Metrics (Large):** Bold, 48-64pt (for highlighting achievements)
- **Body Text:** Regular, 16-18pt
- **Labels/Secondary:** Medium, 14pt
- **Small Stats:** Regular, 12-13pt

**Character:** Rounded, friendly letterforms that feel approachable and non-clinical

## Layout System

**Spacing Units:** Consistent 4pt grid system - commonly use margins/padding of 4, 8, 12, 16, 24, 32

**Screen Structure:**
- Safe area padding: 16-20pt from screen edges
- Section spacing: 24-32pt between major components
- Card internal padding: 16-20pt
- Between related elements: 8-12pt

**Mobile Considerations:**
- Thumb-friendly touch targets (minimum 48x48pt)
- Bottom-heavy navigation for reachability
- Scrollable content with clear visual hierarchy

## Component Library

### Core Navigation
- **Bottom Tab Bar:** 4-5 primary sections (Home, Calendar, Stats, Achievements, Profile)
- Tab icons with labels, active state clearly distinguished
- Fixed at bottom for thumb accessibility

### Home Screen Components
1. **Greeting Card:** Personalized time-of-day greeting with current streak
2. **Quick Log Button:** Prominent CTA for "Going to Sleep" or "Woke Up" based on context
3. **Today's Summary Card:** Sleep duration, quality indicator, points earned
4. **Daily Challenge/Quest Card:** Small gamification element with progress bar
5. **Recent Achievement Badge:** Latest unlocked achievement with celebration micro-animation

### Sleep Calendar View
- **Monthly Grid:** Compact calendar with each day showing sleep quality indicator
- **Day Cards:** Tappable days revealing detailed sleep metrics
- **Week View Toggle:** Alternative horizontal scrolling week view
- **Streak Visualization:** Clear visual indicator of consecutive good sleep days

### Stats Dashboard
1. **Overview Cards Grid:** 2-column layout for key metrics (avg sleep, consistency score, total points)
2. **Sleep Duration Chart:** 7-day or 30-day bar chart showing hours slept
3. **Sleep Quality Trends:** Line graph with quality rating over time
4. **Best Sleep Period:** Highlighted card showing optimal sleep window
5. **Insights Panel:** Automated observations about sleep patterns

### Gamification Elements
- **Points Display:** Always visible in header, animated on earning
- **Achievement Cards:** Grid of locked/unlocked achievements with progress indicators
- **Level Progress Bar:** Shows progress to next level with reward preview
- **Streak Counter:** Prominent display with flame/star icon, celebratory on milestones
- **Daily Quests:** Card-based list with completion checkboxes

### Input Components
- **Time Picker:** Large, easy-to-use circular time selector
- **Sleep Quality Slider:** 5-point scale with emoji indicators (exhausted to refreshed)
- **Notes Input:** Optional text field for sleep notes with character limit
- **Bedtime Goal Setter:** Simple time selection with "Set Reminder" option

### Data Visualization
- **Progress Circles:** For percentage-based metrics (sleep goal completion)
- **Mini Bar Charts:** Inline sparkline charts in summary cards
- **Color-Coded Indicators:** Visual status system for sleep quality (avoid specific color mentions in implementation)
- **Badges:** Small medallion-style icons for achievements

### Modals & Overlays
- **Achievement Unlock Modal:** Full-screen celebration with confetti animation
- **Sleep Log Modal:** Slide-up sheet for logging sleep details
- **Onboarding Flow:** Multi-step introduction with illustration cards
- **Info Tooltips:** Subtle overlay explanations for first-time features

### Buttons & Actions
- **Primary Action Button:** Large, rounded rectangle (min height 54pt) for main CTAs
- **Secondary Buttons:** Outlined style for less critical actions
- **Icon Buttons:** Circular 44x44pt for settings, info, etc.
- **Blurred Button Backgrounds:** When buttons overlay images/illustrations, use frosted glass effect

## Animations & Micro-interactions

**Use Sparingly - Only Where Meaningful:**

1. **Points Earned:** +[number] float-up animation on sleep log submission
2. **Streak Counter:** Pulse effect on daily increment
3. **Achievement Unlock:** Celebratory confetti/particle effect (one-time celebration)
4. **Tab Transitions:** Subtle fade and scale for screen changes
5. **Pull-to-Refresh:** Custom sleep-themed loading animation

**Avoid:** Continuous animations, distracting loops, excessive motion

## Images & Illustrations

### Hero/Welcome Section
- **Onboarding Illustrations:** Custom sleep-themed illustrations showing character in bed, moon/stars, peaceful night scene (3-4 full-screen illustrations for onboarding flow)
- **Empty States:** Friendly illustrations for when no data exists yet (character sleeping peacefully)

### In-App Imagery
- **Achievement Icons:** Stylized icon illustrations for each achievement (moon phases, sleep clouds, stars)
- **Character Avatar:** Simple customizable character that appears in various sleep poses
- **Background Patterns:** Subtle night sky patterns or gradients (non-distracting)

### Image Specifications
- All illustrations should have consistent art style (flat, rounded, friendly)
- SVG format for scalability on different screen densities
- Illustrations should feel calming, not energetic or alarming

## Accessibility

- Minimum touch targets: 48x48pt
- Clear contrast for all text and interactive elements
- Support for system font scaling
- Screen reader labels for all interactive elements
- Haptic feedback for important actions
- Dark mode optimization (critical for sleep app)

## Key Screen Layouts

**Home Screen:** 
- Full-screen scrollable view
- Greeting card at top (1/4 screen height)
- Quick action button (prominent, centered)
- 2-3 summary cards below
- Bottom navigation fixed

**Calendar View:**
- Month grid takes 60% of screen
- Selected day detail panel below
- Header with month navigation

**Stats Screen:**
- Grid of metric cards at top (2x2 grid)
- Full-width charts below
- Scrollable insights section at bottom

**Achievements:**
- Masonry grid of achievement cards
- Progress indicators on locked achievements
- Filter/sort options in header

This design creates an engaging, calming sleep tracking experience that motivates consistent healthy sleep habits through thoughtful gamification.