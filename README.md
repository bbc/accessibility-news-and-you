# BBC News Accessibility
 
The guide used by all members of BBC News development teams to ensure their products meet an excellent standard of accessibility.

## Contributing

Contributions to this guide are welcome! Please submit all contributions as pull requests.

## Testing

To ensure these documents remain up-to-date and in good condition, the following should be done regularly:

- Run a link checker against https://bbc-news.github.io/accessibility-news-and-you/ (the [W3C Link Checker](https://validator.w3.org/checklink) is recommended).
- Review the statistics and recommendations in [_Accessibility and Supported Assistive Technology_](accessibility-and-supported-assistive-technology.md).

## Running the site locally

If you'd like to see your changes locally before committing them, you can get this site running by following these instructions. Note that you'll need Ruby installed for it to run.

- Clone the repository somewhere by running `git clone git@github.com:BBC-News/accessibility-news-and-you.git && cd accessibility-news-and-you`.
- Get all of the dependencies by running `bundle install`.
- Run `bundle exec jekyll serve`. This will watch the files for changes and automatically rebuild.
- Open http://127.0.0.1:4000/ in your web browser.
