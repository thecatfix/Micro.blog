# Micro.blog
Micro.blog repository
[Instructions](https://help.micro.blog/t/archiving-to-github/58)
Micro.blog can automatically copy your posts to a GitHub repository. It uses a similar structure to the Blog Archive Format: an HTML file and JSON Feed of all your blog posts, and an “uploads” folder with all of your photos. Micro.blog will update the archive on GitHub approximately once a week. (If you need an immediate backup, use the Posts → Export feature.)

To enable GitHub archiving, click on Posts → Design and enter a GitHub repository name. Only include the repository name, not a full URL. When you save your blog settings, Micro.blog will prompt you to sign in to your GitHub account if you aren’t signed in, otherwise it will redirect back to Micro.blog with the setting saved.

The repository must be public and must be on the same GitHub account you are signed in as, not a separate GitHub organization. Micro.blog will not have access to any private repositories. Make sure the GitHub repository is not empty. (If it’s a new repository, you can initialize the repository with a README from GitHub.)

To disable archiving and sign out of GitHub, clear the repository name and save your blog settings again from the Posts → Design page.

Micro.blog does not attempt to remove files from your GitHub repository. If you delete an upload from your blog, you’ll need to also delete it manually from GitHub.

If you want GitHub Pages to serve your archive over the web, use a repository name in the format your-username.github.io.


## Custom Domain Names
[Instructions](https://help.micro.blog/t/custom-domain-names/53)
to Micro.blog is included free, as long as you already have your domain registered.

If you don’t have a domain name yet, Micro.blog can handle registering the domain for you. Click on Account → Get a Domain Name. We’ll configure the domain automatically to work with Micro.blog.

To get started with an existing domain name, update your DNS records to point to Micro.blog. Instructions for this will vary depending on your domain registrar, but all registrars will support 2 standard record types: “A” and “CNAME”.

A record → “104.200.22.214”
CNAME record (“www” or “micro”) → “username.micro.blog”
More details:

If you want to use a subdomain such as micro.yourdomain.com or www.yourdomain.com, create a “CNAME” record wherever your domain is registered and use the value “username.micro.blog” (replacing “username” with your own username).
If you want to use a root domain such as yourdomain.com, create an “A” record wherever your domain is registered and use the IP address value: “104.200.22.214”.
If you want both the root domain and www.yourdomain.com to work, you’ll need both an “A” record for the root domain and a “CNAME” record for the “www” version. You can enter either “yourdomain.com” or “www.yourdomain.com” in the Design page settings in Micro.blog.
If you need the IPv6 address, it’s: 2600:3c00:1::68c8:16d6
(Micro.blog will support both the root domain and “www” either way, but what you enter will determine what Micro.blog redirects to if the other domain name is visited. So if you want the root domain without the “www” to be what people see, enter that in the Design page. Micro.blog will then redirect “www” to the root domain.)

After you’ve updated your DNS records, click on Posts → Design in Micro.blog on the web, then scroll down to the custom domain name field. Fill in the hostname (e.g. microblog.yourdomain.com) that you’d like to use for your site.

HTTPS will be enabled automatically for any custom domain.

If you need to register a new domain name, we also offer domain name registration on Micro.blog.

Changing your Domain

As well as adding a custom domain from username.micro.blog to yourdomain.com, you can change to yourotherdomain.com in the future. When adding a custom domain for the first time, or changing to a new one, it may take a few minutes for photos and links to be updated to the new domain.

If you’re using the fediverse support in Micro.blog, after changing your domain name you will need to reset the fediverse username. This effectively “deletes” your account profile from Mastodon servers. Anyone following your Micro.blog account on Mastodon will need to re-follow you.


