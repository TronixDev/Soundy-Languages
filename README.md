# Translations

## How to Add a New Language

1. 📁 Create a new file in the `locales` directory with the name of the language in the format `language_code.json`. For example, `en-US.json` for English, `ms-MY.json` for Melayu and etc.
2. 📋 Copy the contents of the `en-US.json` file into the new file.
3. 🌐 Translate the strings in the new file to the desired language.

## Current Translators

- [x] English (US) - `en-US.json` (Default)
- [x] Indonesian - `id-ID.json` [by @iaMJ](https://github.com/idMJA) 
- [x] Japanese - `ja-JP.json` [by @iaMJ](https://github.com/idMJA) (Not Accurate)
- [x] Polish - `pl-PL.json` [by @JellyTyan](https://github.com/JellyTyan) 

## Translation Rules

1. 🔒 Do NOT translate or modify any text within double curly braces `{{}}`. These are variables that will be replaced with actual values.
   - Example: `"{{prefix}}play"` must stay as `"{{prefix}}play"`
   - Example: `"Page {{current}}/{{total}}"` must stay as `"Page {{current}}/{{total}}"`

2. 🔗 Do NOT translate or modify markdown links `[text](url)`.
   - Example: `[here](https://discord.com/...)` - translate only "here", URL must stay unchanged

3. ✨ Keep all formatting symbols like `**`, `*`, `\n`, etc.
   - Example: `"**Hello!**"` - translate only "Hello", `**` must stay
   - Example: `"Line 1\nLine 2"` - `\n` must stay for line breaks

4. 🎯 Keep the same JSON structure and keys, only translate the values.
   ```json
   {
     "key": "Translate this value",
     "nested": {
       "key": "Translate this value"
     }
   }
   ```

5. 📝 Keep command names exactly as they are.
   - Example: `/play`, `/help`, `/bassboost` must stay unchanged

6. 🚫 Do not add or delete any JSON keys - only translate the values.

7. ✅ Make sure JSON syntax stays valid after translation.
