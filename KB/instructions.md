# How to Create an AI Agent in Microsoft Copilot Studio

This guide provides step-by-step instructions for creating a Copilot agent using **Microsoft Copilot Studio** and adding knowledge sources such as websites and PDF files.

---

## Prerequisites

Before you begin, ensure you have:

- A valid **Microsoft 365** license (or Power Platform license that includes Copilot Studio).
- Access to **[Microsoft Copilot Studio](https://copilotstudio.microsoft.com)**.
- The necessary permissions to create agents in your organization's environment.
- Any website URLs or PDF files you plan to add to the knowledge base.

---

## Part 1 – Create a New Agent

### Step 1: Sign In to Copilot Studio

1. Open your browser and go to **[https://copilotstudio.microsoft.com](https://copilotstudio.microsoft.com)**.
2. Sign in with your **Microsoft work or school account**.
3. Select the appropriate **environment** from the top-right environment picker (e.g., your organization's production or sandbox environment).

---

### Step 2: Create a New Agent

1. On the **Home** screen, click **+ Create** in the left navigation pane, or click the **Create an agent** button on the main canvas.
2. Choose **New agent** from the options presented.
3. You will land on the agent creation form. Fill in the following details:

   | Field | Description |
   |-------|-------------|
   | **Name** | Enter a descriptive name (e.g., *AI Specialization Agent*). |
   | **Description** | Briefly describe what this agent does. |
   | **Instructions** | Provide the agent's core persona and behavior instructions (e.g., "You are a helpful AI specialization assistant for Microsoft partners."). |
   | **Language** | Select the primary language for the agent. |

4. Click **Create** to provision the agent.

---

### Step 3: Configure the Agent's Behavior (Optional)

1. After creation, you will be taken to the agent's **Overview** page.
2. Use the **Topics** section to add conversation topics and trigger phrases if you want to guide specific conversation flows.
3. Use the **Entities** section to define any custom data types the agent should recognize.
4. Use **Actions** to connect the agent to external data or APIs via Power Automate flows (optional, for advanced scenarios).

---

## Part 2 – Add Knowledge Sources

Knowledge sources allow the agent to answer questions based on specific content — such as your documentation websites or uploaded PDF files.

### Step 4: Open the Knowledge Section

1. In the left navigation pane of your agent, click **Knowledge**.
2. You will see the knowledge management panel where you can add and manage sources.

---

### Step 5: Add a Website as a Knowledge Source

1. In the **Knowledge** panel, click **+ Add knowledge**.
2. Select **Public website** from the list of source types.
3. Enter the **URL** of the website you want the agent to use (e.g., `https://learn.microsoft.com/en-us/ai/`).

   > **Tips:**
   > - You can add multiple website URLs, one at a time.
   > - Use URLs that point to publicly accessible pages (the agent cannot access pages behind authentication).
   > - For large documentation sites, prefer linking to specific section URLs rather than the root domain.

4. Click **Add** to confirm.
5. Copilot Studio will crawl and index the website content. Wait for the status to show **Ready** before testing.

---

### Step 6: Add a PDF (File) as a Knowledge Source

1. In the **Knowledge** panel, click **+ Add knowledge**.
2. Select **Files** (or **Upload file**, depending on your Copilot Studio version) from the source type list.
3. Click **Browse** or drag and drop the PDF file(s) you want to upload.

   > **Tips:**
   > - Supported formats include **PDF**, **Word (.docx)**, **PowerPoint (.pptx)**, and **plain text (.txt)**.
   > - The maximum file size per upload is **512 MB**.
   > - Use clearly named files so the agent can reference them accurately.

4. Click **Upload** or **Add** to confirm.
5. Wait for the indexing status to show **Ready**.

---

### Step 7: Verify Knowledge Source Indexing

1. In the **Knowledge** panel, review the list of added sources.
2. Ensure each source shows a status of **✅ Ready** (or **Indexed**).
3. If a source shows an error or **Failed** status:
   - For websites: Check that the URL is publicly accessible and reachable.
   - For files: Ensure the file is not password-protected and is under the size limit.
   - Delete and re-add the source if necessary.

---

## Part 3 – Test the Agent

### Step 8: Test in the Built-in Chat Panel

1. Click the **Test** button (chat bubble icon) in the top-right corner of the Copilot Studio interface to open the test pane.
2. Type a question related to your knowledge sources (e.g., *"What are the AI specialization requirements?"*).
3. Review the agent's response.
   - If the agent answers correctly using knowledge source content, your setup is working.
   - If the response is off-topic or incorrect, review your knowledge sources and agent instructions.
4. Use the **"Reset"** option in the test pane to start a fresh conversation.

---

## Part 4 – Publish the Agent

### Step 9: Publish Your Agent

1. Once you are satisfied with the agent's behavior, click **Publish** in the top-right area of the screen.
2. Confirm the publish action in the dialog that appears.
3. Publishing makes the latest version of your agent available on all configured channels.

---

### Step 10: Share the Agent (Add Channels)

1. Go to the **Channels** section in the left navigation pane.
2. Choose the channel where you want to deploy the agent:

   | Channel | Use Case |
   |---------|----------|
   | **Demo website** | Quick sharing via a hosted webpage link |
   | **Microsoft Teams** | Embed in a Teams app for internal use |
   | **Custom website** | Embed via iframe or Direct Line API |
   | **SharePoint** | Embed in a SharePoint intranet page |

3. Follow the channel-specific instructions to configure and deploy.

---

## Summary

| Step | Action |
|------|--------|
| 1 | Sign in to Copilot Studio |
| 2 | Create a new agent and fill in name, description, and instructions |
| 3 | (Optional) Configure topics, entities, and actions |
| 4 | Open the Knowledge section |
| 5 | Add a website URL as a knowledge source |
| 6 | Upload a PDF or other file as a knowledge source |
| 7 | Verify all sources are indexed and show **Ready** status |
| 8 | Test the agent using the built-in test chat |
| 9 | Publish the agent |
| 10 | Add and configure deployment channels |

---

## Additional Resources

- [Microsoft Copilot Studio Documentation](https://learn.microsoft.com/en-us/microsoft-copilot-studio/)
- [Add knowledge sources in Copilot Studio](https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-sources-overview)
- [Publish your agent to channels](https://learn.microsoft.com/en-us/microsoft-copilot-studio/publication-fundamentals-publish-channels)
- [Microsoft Partner Center – AI Specialization](https://partner.microsoft.com/en-us/membership/ai-specialization)

---

> For an overview of this agent and its intended use for partners, see [readme.md](./readme.md).
