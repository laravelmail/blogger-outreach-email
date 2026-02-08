# Blogger Outreach Email

Professional email template for reaching out to bloggers in the Education and Technology sectors for marketing collaborations.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Technology, Education
- **Message Type:** Marketing
- **Tags:** collaboration, bloggeroutreach

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/blogger-outreach-email.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/blogger-outreach-email/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.blogger-outreach-email',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
