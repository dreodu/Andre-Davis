# Group-5-CMSC-495
CMSC 495 Group5

The starting page for Team ______________.

Insert code outline here:

Input: eml
Output: csv

Sample dictionary built from the features in table 10. This is in Python and would need to be converted into Java's Map instead of the 
Python dictionary.

features_count_dict = {
    #  Boolean values are initialized as None.
    #  Numeric values are initialized to 0.

    #  Feature number 1
    # The number of “Content-Type: multipart/mixed” fields found in the email’s body.
    'Content-Type_multipart/mixed_num': 0,

    #  Feature number 2
    # The number of “Content-Disposition: attachment” fields found in the email’s body.
    'Content-Disposition_attachment_num': 0,

    #  Feature number 3
    # The time span range between the email’s sent and received time.
    'email_span_time': 0,

    #  Feature number 4
    # The number of unique “Content-Transfer-Encoding” fields found in the email’s body.
    'Content-Transfer-Encoding_unique_num': 0,

    #  Feature number 5
    # The number of unique “Content-Disposition” fields found in the email’s body.
    'Content-Disposition_unique_num': 0,

    #  Feature number 6
    # The total number of “Content-Disposition” fields found in the email’s body.
    'Content-Disposition_total_num': 0,

    #  Feature number 7
    # Represents the total size of all attachments found in the email.
    'attachments_total_size_in_bytes': 0,

    #  Feature number 8
    # The number of unique “Content-Type” fields found in the email’s body.
    'Content-Type_unique_num': 0,

    #  Feature number 9
    # The total number of “Content-Transfer-Encoding” fields found in the email’s body.
    'Content-Transfer-Encoding_total_num': 0,

    #  Feature number 10
    # The total number of “Content-Type” fields found in the email’s body.
    'Content-Type_total_num': 0,

    #  Feature number 11
    # The number of unrecognized “Content-Type” fields found in the email’s body.
    'Content-Type_unknown_num': 0,

    #  Feature number 12
    # The unique number of MIME parts found in the email’s body when the email is parsed using the JavaMail library.
    'MimeMessage_Element_unique_num': 0,

    #  Feature number 13
    # The number of characters in the email’s subject.
    'email_subject_length': 0,

    #  Feature number 14
    # The number of characters in the email’s plaintext content.
    'body_plaintext_size': 0,

    #  Feature number 15
    # The number of InputStream type MIME parts found in the email’s body.
    'MimeMessage_Element_InputStream_num': 0,

    #  Feature number 16
    # The number of Multipart type MIME parts found in the email’s body.
    'MimeMessage_Element_Multipart_num': 0,

    #  Feature number 17
    # The number of attachments with content that does not match the file  extension. For example, content of an
    # ∗.exe file with an ∗.txt file extension. Note: this is listed as a boolean in the documentation. There might
    # be a need to fiddle with changing this from a number to a boolean.
    'email_attachments_Mime_Type_Match_Extension_num': 0,

    #  Feature number 18
    #  The number of “Content-Transfer-Encoding: 7bit” fields found in the email’s body.
    'Content-Transfer-Encoding_7bit_num': 0,

    #  Feature number 19
    #  The total number of MIME parts found in the email’s body.
    'MimeMessage_Element_total_num': 0,

    #  Feature number 20
    #  The number of “boundary = ” fields found in the email’s body.
    'email_body_boundaries_num': 0,

    #  Feature number 21
    #  The number of “Content-Type: text/plain” fields found in the email’s body.
    'Content-Type_text/plain_num': 0,

    #  Feature number 22
    #  The version in the “MIME-Version” header field, for example “MIME-Version: 1.0. ”
    'header_MimeVersion': 0,

    #  Feature number 23
    #  Indicates whether the “MIME-Version” field exists in the email’s header.
    'header_exist_MimeVersion': 0,

    #  Feature number 24
    #  The number of URLs that contain a query string found in the email’s body.
    'URL_with_query_string_num': 0,

    #  Feature number 25
    #  The number of attachments that are considered dangerous.
    'attachments_type_Dangerous_num': 0,

    #  Feature number 26
    #  The number of characters in the “MIME-Version” header field.
    'header_MimeVersion_Length': 0,

    #  Feature number 27
    #  The number of text sentences found in the email’s body (consider both plaintext and HTML content).
    'HTML_plaintext_sentences_num': 0,

    #  Feature number 28
    #  The number of “Content-Transfer-Encoding: 8bit” fields found in the email’s body.
    'Content-Transfer-Encoding_8bit_num': 0,

    #  Feature number 29
    #  The number of “Content-Type: multipart/encrypted” fields found in the email’s body.
    'Content-Type_multipart/encrypted_num': 0,

    #  Feature number 30
    #  The number of “Content-Type: …; charset = " iso 2022-jp” fields found in the email’s body.
    'Content-Type-Charset_iso2022-jp_num': 0,

    #  Feature number 31
    #  The number of “Content-Type: …; charset = "us-ascii” fields found in the email’s body.
    'Content-Type-Charset_us-ascii': 0,

    #  Feature number 32
    #  The number of unique charsets found in the email’s body.
    'Content-Type-Charset_unique': 0,

    #  Feature number 33
    #  The number of  iframe  tags in the HTML content.
    'HTML_tag_iframe_num': 0,

    #  Feature number 34
    #  The number of “Content-Transfer-Encoding: binary” fields found in the email’s body.
    'Content-Transfer-Encoding_binary_num': 0,

    #  Feature number 35
    #  The number of “Content-Type: multipart/signed” fields found in the email’s body.
    'Content-Type_multipart/signed_num': 0,

    #  Feature number 36
    #  The number of unique domains found in URLs in the email’s body.
    'email_body_domains_URL_unique_num': 0,

    #  Feature number 37
    # The number of URLs found in the email’s body.
    'Email_body_URLs_num': 0,

    #  Feature number 38
    #  The number of unique domains found in the email.
    'email_body_domains_unique_num': 0,

    #  Feature number 39
    #  The total number of charsets found in the email’s body.
    'Content-Type-Charset_total': 0,

    #  Feature number 40
    #  The number of attachments that belong to the video category (e.g., ∗.mp4, ∗.avi, etc.).
    'attachments_type_Video_num': 0,

    #  Feature number 41
    #  The number of attachments that belong to the image category (e.g., ∗.jpg, ∗.png, etc.).
    'attachments_type_Image_num': 0,

    #  Feature number 42
    #  The number of attachments that belong to the digital signature category (e.g., ∗.p7s).
    'attachments_type_DigitalSignature_num': 0,

    #  Feature number 43
    #  The number of MIME parts found in the email’s body that cause an error when parsing
    #  with the JavaMail package.
    'MimeMessage_Element_error': 0,

    #  Feature number 44
    #  The number of unknown or non-standard “Content-Transfer-Encoding” values.
    'Content-Transfer-Encoding_unknown': 0,

    #  Feature number 45
    #  The number of attachments that are part of the text category (e.g., ∗.txt, ∗.xml, ∗.csv).
    'attachments_type_Text_num': 0,

    #  Feature number 46
    #  The number of “Content-Type: multipart/related” fields found in the email’s body.
    'Content-Type_multipart/related': 0,

    #  Feature number 47
    #  The number of <link> tags in the HTML content.
    'HTML_with_tag_link': 0,

    #  Feature number 48
    #  The number of unrecognized attachment types.
    'attachments_type_Unrecognized_num': 0,

    #  Feature number 49
    #  The number of email addresses found in the email’s body.
    'email_body_Email_Addresses_num': 0,

    #  Feature number 50
    #  The length of the header part of the email in byes.
    'email_headers_length': 0,

    #  Feature number 51
    #  The number of “Content-Type: …; charset = "utf-8  fields found in the email’s body.
    'Content-Type-Charset_utf-8': 0,

    #  Feature number 52
    #  The number of URLs in the email body that are related to URL shortening services (e.g., bitly, goo.gl, etc.).
    'URL_Short_Service_num': 0,

    #  Feature number 53
    #  The number of “Content-Type: multipart/report” fields found in the email’s body.
    'Content-Type_multipart/report': 0,

    #  Feature number 54
    #  The number of “References” headers.
    'header_Reference_num': 0,

    #  Feature number 55
    #  The number of headers found in the email’s header.
    'email_headers_num': 0,

    #  Feature number 56
    #  The number of “Content-Transfer-Encoding: quoted-printable” fields
    'Content-Transfer-Encoding_quoted-printable': 0,

    #  Feature number 57
    #  The number of unrecognized charsets found in the email’s body.
    'Content-Type-Charset_unknown_num': 0,

    #  Feature number 58
    #  The number of unique domain names found in the email.
    'email_body_domains_EmailAddresses_unique_num': 0,

    #  Feature number 59
    #  The number of different languages found in the email’s body text. The languages are determined using the
    #  Tika Java package -> use pipy's tika (will have to search for the equivalent methods)
    'body_plaintext_languages_num': 0,

    #  Feature number 60
    #  The number of “Content-Type: text/html” fields found in the email’s body.
    'Content-Type_text/html_num': 0,

    #  Feature number 61
    #  The number of headers in which the name is not in the correct case.
    #  For example: "MIME-Version" vs "Mime-Version".
    'email_headers_incorrect_name_num': 0,

    #  Feature number 62
    #  The number of “Content-Type: multipart/alternative” fields found in the email’s body.
    'Content-Type_multipart/alternative': 0,

    #  Feature number 63
    #  Indicates whether the “X-Spam-Status” field exists in the email’s header.
    'header_exist_XSpamStatus': None,

    #  Feature number 64
    #  The number of “Content-Type: …; charset = "gb2312” fields found in the email’s body.
    'Content-Type-Charset_gb2312_num': 0,

    #  Feature number 65
    #  The number of “Content-Disposition: inline” fields found in the email’s body.
    'Content-Disposition_inline_num': 0,

    #  Feature number 66
    #  The number of “Content-Type: …; charset = "shift-jis” fields found in the email’s body.
    'Content-Type-Charset_shift_jis_num': 0,

    #  Feature number 67
    #  The number of MimeMessage parts found in the email’s body.
    'MimeMessage_Element_MimeMessage_num': 0,

    #  Feature number 68
    #  The number of “Content-Type: message/rfc822” fields found in the email’s body.
    'Content-Type_message/rfc822_num': 0,

    #  Feature number 69
    #  The number of “Content-Type: …; charset = "utf-7  fields found in the email’s body.
    'Content-Type-Charset_utf-7_num': 0,

    #  Feature number 70
    #  The number of forward strings (Forward/Fw:) found in the email’s subject.
    'email_subject_contains_forward_string_num': 0,

    #  Feature number 71
    #  The number of reply strings (Reply/ Re :) found in the email’s subject.
    'email_subject_contains_reply_string_num': 0,

    # Feature number 72
    #  The number of senders in the “From” header.
    'header_From_senders_num': 0,

    #  Feature number 73
    #  The number of images in HTML that function as links.
    'HTML_link_image_num': 0,

    #  Feature number 74
    #  The number of attachments that belong to the audio category (e.g., ∗.mp3, ∗.wav, etc.).
    'attachments_type_Audio_num': 0,

    #  Feature number 75
    #  The number of MIME parts from String type, found in the email’s body.
    'MimeMessage_Element_String_num': 0,

    #  Feature number 76
    #  Indicates whether the email address in the "From” header field complies with the standards set
    #  by the Internet RFCs.
    'header_From_EmailAddress_is_Valid': None,

    #  Feature number 77
    #  Indicates whether the email is a no-reply email.
    'email_no_reply': None,

    #  Feature number 78
    #  Indicates whether the domains in the “From” and the “Reply-To” headers are similar.
    'header_domain_similarity_From_x_ReplyTo': None,

    #  Feature number 79
    #  The number of encoded URLs (may contain characters in languages other than English).
    'URL_encoded_num': 0,

    #  Feature number 80
    #  Indicates the importance of an email (1 = Low, 2 = Medium, 3 = High).
    'header_Importance': 0,

    #  Feature number 81
    #  The number of URLs with percent encoding https://en.wikipedia.org/wiki/Percent-encoding
    #  (i.e., contains “%XW%YZ,)
    'URL_with_percent_encoding_num': 0,

    #  Feature number 82
    #  Indicates whether the “Importance” header exists.
    'header_exist_Importance': None,

    #  Feature number 83
    #  The number of attachments with no file extension found in the email.
    'attachments_type_NoExtension_num': 0,

    #  Feature number 84
    #  The number of unrecognized “Content-Disposition” fields found in the email’s body.
    'Content-Disposition_unknown_num': 0,

    #  Feature number 85
    #  The number of FTP URLs.
    'URL_FTP_num': 0,

    #  Feature number 86
    #  The number of non-English characters in URLs observed in the email.
    'URL_Non_English_Characters': 0,

    #  Feature number 87
    #  The number of abnormal links in HTML. We define abnormal as transparent links with a text similar to the
    #  background. Such links are invisible to the reader’s eye and used for usually for malicious purposes.
    'HTML_link_abnormal_num': 0,

    #  Feature number 88
    #  The number of “Content-Type: multipart/digest” fields found in the email’s body.
    'Content-Type_multipart/digest_num': 0,

    #  Feature number 89
    #  The number of “Content-Type: …; charset = "cp-850  fields found in the email’s body.
    'Content-Type-Charset_cp-850_num': 0,

    #  Feature number 90
    #  Indicates whether the header “Subject” exists in the email’s header.
    'header_exist_Subject': None,

    #  Feature number 91
    #  The number of “Content-Type: multipart/byterange” fields found in the email’s body.
    'Content-Type_multipart/byterange_num': 0,

    #  Feature number 92
    #  The number of “Content-Type: multipart/form-data” fields found in the email’s body.
    'Content-Type_multipart/form-data_num': 0,

    #  Feature number 93
    #  The number of “Content-Type: multipart/parallel” fields found in the email’s body.
    'Content-Type_multipart/parallel_num': 0,

    #  Feature number 94
    #  The number of “Content-Type: multipart/x-mixed-replaced” fields found in the email’s body.
    'Content-Type_multipart/x-mixed-replaced_num': 0,

    #  Feature number 95
    #  The number of “Content-Type: …; charset = " iso 8859  fields found in the email’s body.
    'Content-Type-Charset_iso8859_num': 0,

    #  Feature number 96
    #  The number of “Content-Type: …; charset = "koi” fields found in the email’s body.
    'Content-Type-Charset_koi_num': 0,

    #  Feature number 97
    # The number of “Content-Type: …; charset = "windows-12  fields found in the email’s body.
    'Content-Type-Charset_windows-12_num': 0,

    #  Feature number 98
    #  The number of “Content-Type: …; charset = "x-sjis” fields found in the email’s body.
    'Content-Type-Charset_x-sjis_num': 0,

    #  Feature number 99
    #  The number of recipients in the “Error-To” header.
    'header_recipients_ErrorTo_num': 0,

    #  Feature number 100
    #  The number of unrecognized MimeMessage elements found in the email.
    'MimeMessage_Element_unknown_num': 0

}


