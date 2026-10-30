# Challenge: Sunrise Community Clinic opening hours

Build a one-page website for a **fictional** clinic. All the information is in `src/data.json`.
Build it in `src/App.tsx` (you may add more components). `App` must stay the **default export**.

Use the **exact words** shown in quotes below: the checker looks for them.

## Requirements

1. **Heading.** The page has one main heading (`h1`) showing the clinic name from `data.json`: "Sunrise Community Clinic".
2. **Opening hours.** Show a list labelled "Opening hours" (`aria-label="Opening hours"`) with 7 items, Monday to Sunday in that order. Each item reads like "Monday: 08:00-18:00" (day, colon, space, open time, hyphen, close time). A day with no hours reads "Sunday: Closed".
3. **Today.** The item for today's day of the week is highlighted (bold or coloured) and has `aria-current="date"`. No other item has it.
4. **Open now?** Show "Open now" if the current time is between today's open time (included) and close time (not included). Otherwise show "Closed now".
5. **Services.** Show a list labelled "Services" (`aria-label="Services"`) with one item per service, showing the service name.
6. **Search.** A text box labelled "Search services" filters the Services list as you type. It matches any part of the name and ignores upper or lower case (for example "BLOOD" shows "Blood pressure check" and "Blood test").
7. **No results.** When nothing matches, the Services list is empty and the page shows "No services found".
8. **Category filter.** A drop-down labelled "Category" has the options "All", "Adults", "Vaccines", "Children" and "Tests". Choosing a category shows only that category's services. Search and category work together.
9. **Call us.** A link with the text "Call us" opens the phone dialler: `href="tel:+1-555-0100"` (the phone number from `data.json`).
10. **Disclaimer.** The page shows this exact sentence: "This is a fictional clinic for practice. It does not give medical advice."

## Tips

- Ask Claude for a plan first, then let it build one requirement at a time.
- Run `npm run dev` (ask Claude) and open the link to look at your page.
- Make it look good with Tailwind CSS classes, but finish the requirements first.
