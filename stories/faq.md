<!-- 
.. title: Frequently Asked Questions
.. slug: faq
.. date: 2016-10-03 05:16:01 UTC-05:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

-   [Where can I find the latest version of TW Blue?](#download)
-   [How often are new versions released?](#new_versions)
-   [After updating TW Blue, the application fails to start. What do I
    do?](#update_issues)
-   [I have another Twitter client that also has an invisible interface.
    Can I use it at the same time as TW Blue’s invisible
    interface?](#multiple_hidden_windows)
-   [How can I force TW Blue to update timeline
    buffers?](#updating_buffers)
-   [Can I use the translation function of TW Blue to communicate with
    people in other countries](#translating)
-   [Can I use more than one Twitter account with TW
    Blue?](#more_than_one_account)
-   [I have an API key for Sndup but my audio files will not upload,
    even though I put it in the configuration dialog. Why?](#api_key)
-   [I would like to help with the TW Blue project. How can I get
    involved?](#help)

Where can I find the latest version of TW Blue? {#download}
-----------------------------------------------

The latest version of TW Blue can always be downloaded from our
[download page.](download.en.html) You will be able to download the
appropriate version for your architecture (either 32 or 64-bit). Keep in
mind that the program checks for new versions automatically; so if you
already have it installed, you will be notified when a new version is
available. It is recommended that the automatic update process be used
as installing new versions is as simple as pressing “Yes” in the update
notification dialog. The program will then download the new version and
install it automatically.

How often are new versions released? {#new_versions}
------------------------------------

At the start of TW Blue’s development, a new version of the program was
released every Saturday. Fortunately, however, the project has grown but
this also means that the code has become more complex. This has made it
impossible to continue releasing new versions weekly and, at this point
in time, there is no fixed release schedule. We wish to insure that all
new features work as intended upon release and that there are no
unexpected errors. You can follow our Twitter account
[@tw\_blue2](https://twitter.com/tw_blue2) and we will let you know as
soon as a new version is available. Also, your installed copy of TW Blue
will notify you.

After updating TW Blue, the application fails to start. What do I do? {#update_issues}
---------------------------------------------------------------------

If TW Blue fails to run after an update, please try the following:

-   Download the new version again from the web site.
-   Unzip the newly downloaded version in a folder that has no accent
    marks in its name. This folder should also be empty and separate
    from the one containing the version of TW Blue that is not working.
-   Next, copy the config folder from the version that is not working
    into the folder containing the fresh copy.
-   Now, try to start the program.
-   If it still won’t run, delete the config folder and repeat
    the process. The client will ask you to authorize through the
    Twitter web site.
-   If all else fails, please file a bug report and include the content
    of the following files: logs/tracebacks.log, logs/debug.log
    and logs/error.log.

I have another Twitter client that also has an invisible interface. Can I use it at the same time as TW Blue’s invisible interface? {#multiple_hidden_windows}
-----------------------------------------------------------------------------------------------------------------------------------

No. Due to the fact that some characteristics of these programs are the
same, this is impossible. If you were to attempt doing this, the
keystrokes of the second invisible client will superceed those of the
first. The first client will become unusable and you will have to kill
its process.

How can I force TW Blue to update timeline buffers? {#updating_buffers}
---------------------------------------------------

the short answer is that you can’t. The more complicated answer is that
TW Blue works differently than other Twitter clients, which retrieve new
tweets periodically.

When you start TW Blue, all tweets will be downloaded and the program
will say, “Ready” as well as play a sound when it is done. From this
point onward, as soon as a tweet, mention, direct message or follow
request comes to your account, it will be recognized immediately by TW
Blue. If, however, the connection is dropped, TW Blue will reconnect to
Twitter and download all tweets that were missed as soon as a connection
to the internet is available again. All events are handled in realtime,
so there is no need to force an update.

Can I use the translation function of TW Blue to communicate with people in other countries? {#translating}
--------------------------------------------------------------------------------------------

No. Translation is handled by [Google
Translate](http://translate.google.com) which itself states that a
machine translation will never match the accuracy of that produced by a
human translator. Of course, the final decision rests with the user. If
you feel that Google Translate is sufficient for what you are trying to
accomplish, then by all means use it.

Can I use more than one Twitter account with TW Blue? {#more_than_one_account}
-----------------------------------------------------

This is currently not supported. You can, however, install a separate
copy of TW Blue into a different folder and configure it to use your
other Twitter client. You will then have two instances of the program
running, with a window for each. Keep in mind, though, that you can only
activate invisible mode on one of these instances. Also, to avoid
confusion between applications, insure that no other program is running
that uses the same keystrokes as TW Blue’s invisibility mode.

I have an API key for Sndup which I have entered in TW Blue’s preferences dialog, but my audio files still won’t upload. Why? {#api_key}
-----------------------------------------------------------------------------------------------------------------------------

Please check the following:

1.  TW Blue can attach files anonymously.
2.  Make sure that the API key in TW Blue’s preferences dialog is
    exactly the same as the one in your profile at
    [SndUp.](http://sndup.net) Double check that you haven’t left any
    spaces or newline characters in the key by mistake.

If you’ve followed the above suggestions and are still encountering
problems, please report it through the “Report an error” option in the
Help menu.

I would like to help with the TW Blue project. How can I get involved? {#help}
----------------------------------------------------------------------

If you enjoy using TW Blue and you’d like to help make it better, there
are many things you can do. Any help you can offer is welcome. Here are
a few ways in which you can help with the development of TW Blue:

-   Report all errors that you find with the behavior of the application
    under your specific platform. This can be done using the “Report an
    error” option in the help menu. Please provide contact details so
    that we can follow up for more specific information about the error.
-   Also, donations of any amount are welcome and can be made through
    our [donation page.](donate.en.html) This will help us focus more
    time and effort into development of TW Blue.
-   If you like the application, you can also help out by recommending
    it to your friends and others through your social networks.
-   If you maintain a web site or blog, it would be fantastic if you
    could spread the word by writing about the program. Ideas and
    constructive criticism are accepted with open arms.
-   If you are proficient in other languages and would like to help make
    TW Blue available to more people throughout the world, please
    contact us at [info@twblue.com.mx](info@twblue.com.mx) to submit
    your translation.
-   If you can program in [Python](http://python.org) and [WX
    Python](http://wxpython.org) or any other programming languages and
    you are interested in contributing to the development of TW Blue,
    get in touch with us to see what we can work out.