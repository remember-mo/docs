<!--
This file is auto-generated and will be re-generated every time the docs are updated.
To modify it, go to its source at https://github.com/fastlane/fastlane/blob/master/fastlane/lib/fastlane/actions/mailgun.rb
-->

# mailgun


Send a success/error message to an email group







mailgun ||
---|---
Supported platforms | ios, android, mac
Author | @thiagolioy



## 2 Examples

```ruby
mailgun(
  to: "fastlane@krausefx.com",
  success: true,
  message: "This is the mail's content"
)
```

```ruby
mailgun(
  postmaster: "MY_POSTMASTER",
  apikey: "MY_API_KEY",
  to: "DESTINATION_EMAIL",
  from: "EMAIL_FROM_NAME",
  reply_to: "EMAIL_REPLY_TO",
  success: true,
  message: "Mail Body",
  app_link: "http://www.myapplink.com",
  ci_build_link: "http://www.mycibuildlink.com",
  template_path: "HTML_TEMPLATE_PATH",
  custom_placeholders: {
    :var1 => 123,
    :var2 => "string"
  },
  attachment: "dirname/filename.ext"
)
```





## Parameters

Key | Description | Default
----|-------------|--------
  `mailgun_sandbox_domain` | Mailgun sandbox domain postmaster for your mail. Please use postmaster instead | 
  `mailgun_sandbox_postmaster` | Mailgun sandbox domain postmaster for your mail. Please use postmaster instead | 
  `mailgun_apikey` | Mailgun apikey for your mail. Please use postmaster instead | 
  `postmaster` | Mailgun sandbox domain postmaster for your mail | 
  `apikey` | Mailgun apikey for your mail | 
  `to` | Destination of your mail | 
  `from` | Mailgun sender name | `Mailgun Sandbox`
  `message` | Message of your mail | 
  `subject` | Subject of your mail | `fastlane build`
  `success` | Was this build successful? (true/false) | `true`
  `app_link` | App Release link | 
  `ci_build_link` | CI Build Link | 
  `template_path` | Mail HTML template | 
  `reply_to` | Mail Reply to | 
  `attachment` | Mail Attachment filenames, either an array or just one string | 
  `custom_placeholders` | Placeholders for template given as a hash | `{}`

<em id="parameters-legend-dynamic">* = default value is dependent on the user's system</em>


<hr />
To show the documentation in your terminal, run
```no-highlight
fastlane action mailgun
```

<a href="https://github.com/fastlane/fastlane/blob/master/fastlane/lib/fastlane/actions/mailgun.rb" target="_blank">View source code</a>

<hr />

<a href="/actions"><b>Back to actions</b></a>
