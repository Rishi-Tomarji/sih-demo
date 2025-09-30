# Educational Tech Platform - Design Guidelines

## Design Approach

**Selected Approach:** Design System Foundation with Educational Enhancement
- **Base System:** Material Design 3 principles for clarity and accessibility
- **Reference Inspiration:** Khan Academy (learning focus), Duolingo (engagement), Google Classroom (organization)
- **Key Principle:** Create an interface that feels professional for teachers while remaining approachable and engaging for students

## Color Palette

### Light Mode
- **Primary (Brand):** 217 91% 60% (Blue - trust, learning)
- **Secondary (Accent):** 142 71% 45% (Green - success, growth)
- **Background:** 0 0% 98%
- **Surface:** 0 0% 100%
- **Text Primary:** 220 13% 18%
- **Text Secondary:** 220 9% 46%

### Dark Mode
- **Primary:** 217 91% 70%
- **Secondary:** 142 76% 55%
- **Background:** 220 13% 10%
- **Surface:** 220 13% 15%
- **Text Primary:** 0 0% 98%
- **Text Secondary:** 220 9% 70%

### Semantic Colors
- **Success:** 142 71% 45%
- **Warning:** 38 92% 50%
- **Error:** 0 72% 51%
- **Info:** 199 89% 48%

## Typography

**Font Stack:**
- **Primary:** 'Inter' (Google Fonts) - body text, UI elements
- **Display:** 'Poppins' (Google Fonts) - headings, emphasis

**Scale:**
- Headings: text-4xl/font-bold (Dashboard titles), text-2xl/font-semibold (Section headers), text-xl/font-semibold (Card titles)
- Body: text-base (Primary content), text-sm (Secondary info, captions)
- UI: text-sm/font-medium (Buttons, labels)

## Layout System

**Spacing Primitives:** Tailwind units of 3, 4, 6, 8, 12, 16
- Consistent spacing creates rhythm: p-4, gap-6, m-8, py-12, px-16
- Card padding: p-6
- Section spacing: py-12 or py-16
- Grid gaps: gap-4 or gap-6

**Container Strategy:**
- Dashboard max-width: max-w-7xl mx-auto
- Content cards: full-width within containers
- Forms: max-w-2xl for optimal readability

## Component Library

### Navigation
- **Top Navigation Bar:** Fixed header with logo, search bar, profile dropdown, and notifications
- **Student Nav:** Includes Home, My Courses, Quizzes, Puzzles, Progress icons
- **Teacher Nav:** Dashboard, Students, Create Content, Analytics, Settings
- **Design:** Clean horizontal nav with active state indicators (border-b-2 for active items)

### Dashboard Cards
- **Content Cards:** Rounded corners (rounded-xl), shadow-md, hover:shadow-lg transition
- **Continue Watching:** Horizontal scroll cards with thumbnail, title, progress bar
- **Subject Cards:** Grid layout with subject icon, name, lesson count
- **Student Progress Cards:** Data visualization with charts, percentages, status badges

### Profile Components
- **Profile Header:** Large avatar (w-24 h-24), username, role badge
- **Edit Profile Form:** Two-column layout on desktop (grid-cols-2), single column mobile
- **Profile Picture Upload:** Circular frame with edit overlay on hover

### Content Rows
- **Horizontal Scrollers:** overflow-x-auto with snap-x snap-mandatory for smooth scrolling
- **Card Design:** Consistent aspect ratio, thumbnail on top, text below
- **Spacing:** gap-4 between cards, pr-4 on container for breathing room

### Quiz/Puzzle Interface
- **Quiz Cards:** Clean question cards with multiple choice buttons, progress indicator at top
- **Timer Display:** Top-right corner with visual countdown (if applicable)
- **Results Screen:** Celebratory design with score, correct/incorrect breakdown, retry button

### Data Tables (Teacher Portal)
- **Student Data Tables:** Sortable columns, search filter, pagination
- **Design:** Striped rows (bg-gray-50 dark:bg-gray-800/50), hover states
- **Action Buttons:** Icon buttons for quick actions (view, edit, delete)

### Forms
- **Input Fields:** Consistent height (h-12), rounded-lg borders, focus:ring-2 focus:ring-primary
- **Labels:** text-sm font-medium, mb-2 spacing
- **Validation:** Inline error messages in error color with icon

### Login Page
- **Layout:** Centered card on gradient background
- **Card Design:** max-w-md, p-8, rounded-2xl, shadow-2xl
- **Role Selection:** Toggle or tab interface for Student/Teacher selection
- **CTA Button:** Full-width, prominent primary color

### Buttons
- **Primary:** bg-primary text-white, px-6 py-3, rounded-lg
- **Secondary:** border-2 border-primary text-primary, px-6 py-3, rounded-lg
- **Icon Buttons:** p-2, rounded-lg, hover:bg-gray-100

## Images

### Hero/Feature Images
- **Login Page:** Abstract educational illustration or geometric pattern background (gradient overlay 217 91% 60% to 142 71% 45%)
- **Dashboard Empty States:** Playful illustrations for empty quiz sections, no courses yet
- **Subject Icons:** Colorblind-friendly icon set for Math, Science, Technology, Engineering (use Heroicons or Material Icons)
- **Profile Placeholders:** Default avatars with initial letters on colored backgrounds

### Placement
- Login background: Full-screen with overlay
- Dashboard: Profile pictures, course thumbnails (16:9 ratio), achievement badges
- No large hero images on dashboard pages - focus on content density

## Accessibility Features

- **Colorblind Modes:** Pattern overlays on charts, icons alongside colors
- **Contrast Ratios:** Minimum 4.5:1 for normal text, 3:1 for large text
- **Focus Indicators:** Clear 2px ring on all interactive elements
- **Screen Reader:** Semantic HTML, proper ARIA labels, descriptive alt text
- **Keyboard Navigation:** Full keyboard support, logical tab order
- **Text Size Controls:** User preference for increasing font sizes

## Animations

**Minimal and Purposeful:**
- Card hover: transform scale-105 transition-transform duration-200
- Page transitions: Smooth fade (opacity changes only)
- Progress bars: Animated width changes with ease-out
- Loading states: Simple spinner or skeleton screens
- **Avoid:** Excessive motion, distracting effects

## Dashboard-Specific Design

### Student Dashboard
- **Visual Hierarchy:** Profile section → Quick actions → Content rows
- **Content Density:** Moderate - balance between information and whitespace
- **Engagement Elements:** Progress visualizations, achievement badges, streak counters

### Teacher Dashboard
- **Data Focus:** Charts, tables, analytics front and center
- **Action-Oriented:** Quick create buttons, batch actions, filters
- **Professional Tone:** Clean, organized, information-dense without clutter

This comprehensive design system creates an educational platform that's both functional and engaging, with careful attention to accessibility and user experience for both student and teacher personas.