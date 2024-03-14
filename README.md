Installation:

In the head section:
<link href="style_tags.css" rel="stylesheet" type="text/css">
<script src="scripTags.js"></script>

Code in html:
<input type=text name="text" value="value1, value2, ..."> // the value is optional, separated by a comma by default
<div class="field-tags-list">
            <div class="itemtag">word1</div>
            <div class="itemtag">word2</div>
            <div class="itemtag">word3</div>
            .... // more
</div>

<script>
    const config = { 
      inputName: "tags_name",
      fieldDrop: ".field-tags-list .itemtag",
    };
    const tags = new Tags(config);
</scirpt>

Default configuration: 
 
 config = {
            inputName: "email", // name of the input we want to replace
            fieldDrop: ".field-tags-list .itemtag", // values that are available for inputTagDrop
            separate: ', ',     // data separator to send
            type: "default",    // validation type (mail, text)
            limit: 512          // total string length limit O or null no limit
        };
  lang = 'pl'; // language version (pl, en, de, ru, hu)
  tagas = new Tags(config, lang)
