## Usage Guide

### 1. Generate Prompt Database
**File:** `generate-prompts.html`

This tool fetches exercise data and creates detailed visual descriptions (camera angle, movement arrows, badges).

1.  **Open** `generate-prompts.html` in a web browser.
2.  **Fetch Data:** Click **Fetch & Generate JSON**.
    * *Configuration:* Toggle **Generate for all exercises** to process the full dataset. Uncheck to limit to the first 50 exercises for faster testing.
3.  **Export:** Click **Download JSON** to save the `exercise-prompts.json` file locally.

### 2. Generate Images
**File:** `generate-images.html`

This tool consumes the JSON metadata to generate the final images.

1.  **Open** `generate-images.html` in a web browser.
2.  **Load Data:**
    * Locate the **Load Local JSON** section.
    * Upload the `exercise-prompts.json` file generated in Step 1.
    * Click **Load Local JSON**.
3.  **Configure Settings:**
    * **Test Mode:** Uncheck this to enable real AI generation (requires Puter authentication). Leave checked to generate grey placeholders without using credits.
    * **Use embedded prompts:** **Must be checked**. This forces the tool to use the detailed descriptions created in Step 1.
    * **Omit Labels:** Check this to remove the "Phase" badges and text overlays from the output images.
4.  **Select & Run:**
    * Select specific exercises from the list or click **Select All Visible**.
    * Click **Generate Selected Images**.
5.  **Save:**
    * Click **Download All Images** to save the resulting PNGs.
    * (Optional) Click **Download Generated Metadata JSON** to save the mapping file.
