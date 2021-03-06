# DSTC6_Track2_Information-End-to-End-Conversation-Modeling

1. Main task (mandatory): Customer service dialog using Twitter

    (*) The tools to download the twitter data and transform to the dialog format from the data are provided.


    Task A: Full or part of the training data will be used to train conversation models.

    Task B: Any open data, e.g. from web, are available as external knowledge to generate informative sentences. But they should not overlap
with the training, validation and test data provided by organizers.

2. Pilot task: Movie scenario dialog using OpenSubtitle

# Necessary steps

The tools and data sets are available for the DSTC6 attendees. 
Please visit the following page to make your registration.

    http://workshop.colips.org/dstc6/index.html

We will provide the access token to download the tools and data sets.

## Twitter task

1. prepare data set using collect_twitter_dialogs scripts.

    (see collect_twitter_dialogs/README.md)

2. extract training and development sets from stored twitter dialog data

    use make_trial_data.sh in tasks/twitter.

    Note: the extracted data are trial data at this moment.

3. run baseline system (optional)

    copy the data files into ChatbotBaseline/egs/twitter and
    execute 'run.sh' in ChatbotBaseline/egs/twitter.
    (see ChatbotBaseline/egs/twitter/README.md)

## OpenSubtitles task

1. download OpenSubtitles2016 data:

    http://opus.lingfil.uu.se/download.php?f=OpenSubtitles2016/en.tar.gz

    and extract xml files by

    $ tar zxvf en.tar.gz

2. extract training and development sets from stored subtitle data

    use make_trial_data.sh in tasks/opensubs.

    Note: the extracted data are trial data at this moment.

3. run baseline system (optional)

    copy the data files into ChatbotBaseline/egs/opensubs and
    execute 'run.sh' in ChatbotBaseline/egs/opensubs.

    (see ChatbotBaseline/egs/opensubs/README.md)

## Directories and files
- README.md : this file
- tasks : data preparation for each subtask
- collect_twitter_dialogs : scripts to collect twitter data
- ChatbotBaseline : a neural conversation model baseline system

## Contac Information 
You can get the latest updates and participate in discussions on DSTC mailing list

To join the mailing list, send an email to: (listserv@lists.research.microsoft.com) putting "subscribe DSTC" in the body of the message (without the quotes). To post a message, send your message to: (dstc@lists.research.microsoft.com).
