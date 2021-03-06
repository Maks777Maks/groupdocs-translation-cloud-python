# GroupDocs Translation Cloud 

[GroupDocs.Translation Cloud](https://products.groupdocs.cloud/translation) is Cloud API to translate Word and Excel files as well as plain text. 

For convenience of our Python customers we introduce a simple SDK used to add translation of Microsoft Word documents, Microsoft Excel workbooks and plain text to your app with merely a few lines of code.

In detail, it's a set of SDKs for document and plain text translation in our Cloud. It supports translaton of .doc, .docx, .docm, .xls, .xlsx, .xlsm files. Just pass a specific file or text to the GroupDocs.Translation Cloud API, and it will translate and save translated file in our Cloud or will return translated text.

It is easy to get started with GroupDocs.Translation Cloud, and there is nothing to install. Create an account at [GroupDocs Cloud](https://dashboard.aspose.cloud/#/) and get your application information, then you are ready to use [SDKs](https://github.com/groupdocs-translation-cloud)

## Release 20.9
- French-German language pair support

## Release 20.8:
- GroupDocs.Translation Cloud Python SDK


## Features:

- Translation of Microsoft Word and Microsoft Excel documents
- [10 languages and 20 languages pairs support](https://docs.groupdocs.cloud/translation/supported-languages/)
- Translation of tables, headers, footers, footnotes / endnotes, image captions in Word documents
- Translation of cells, charts, tables, pivot tables in Excel documents
- Translation of plain text
- API that allows you manage your files and folders in our Cloud

## How to use the SDK?

Our API is completely independent of your operating system, database system, or development language. You can use any language and platform that supports HTTP to interact with our API. However, manually writing client code can be difficult, error-prone, and time-consuming. Therefore, we have provided and support [SDKs](https://github.com/groupdocs-translation-cloud) in many development languages to make it easier to integrate with us.

## Examples

```python
from groupdocstranslationcloud.configuration import Configuration
from groupdocstranslationcloud.api.translation_api import TranslationApi
from groupdocstranslationcloud.models.translate_text import TranslateText
from groupdocstranslationcloud.models.translate_document import TranslateDocument

#enter valid apiKey and appSid
configuration = Configuration(apiKey="", appSid="")
api = TranslationApi(configuration)

# text translation
pair = "en-fr"
text = "Welcome to Paris"
translator = TranslateText(pair, text)
request = translator.to_string()
res_text = api.post_translate_text(request)
print(res_text.translation)

#document translation
pair = "en-fr"
_format = "docx"
storage = "First Storage"
name = "test.docx"
folder = ""
savepath = ""
savefile = "test_python.docx"  
translator = TranslateDocument(pair, _format, storage, name, folder, savepath, savefile)
request = translator.to_string() 
res_doc = api.post_translate_document(request)
print(res_doc.message)
```
_________________________

## Quickstart

Make your solution using [SDK](https://github.com/groupdocs-translation-cloud), follow these steps:

#### 1. Get API keys if you haven't

Make a personal account on [GroupDocs Cloud Dashboard](https://dashboard.groupdocs.cloud/#/) and click _Get Keys_. These keys are useful for all GroupDocs Cloud products. If you have any trouble, look at this [detailed manual](https://docs.groupdocs.cloud/translation/create-new-app-and-get-app-key-and-sid).

#### 2. Install SDK

Install `groupdocs-translation-cloud` with [PIP](https://pypi.org/project/pip/) from [PyPI](https://pypi.org/) by:

```sh
pip install groupdocs-translation-cloud
```

Or clone repository and install it via [Setuptools](http://pypi.python.org/pypi/setuptools): 

```sh
python setup.py install
```

#### 3. Run Demo

  * Checkout the SDK or get from PiPy 
  * Set Your AppSid & AppKey
  * Run Jupyter Notebook [demo.ipynb](https://github.com/groupdocs-translation-cloud/groupdocs-translation-cloud-python/blob/master/demo.ipynb)
 
--------------------------- 

### Structure

This project includes:

- Module "groupdocstranslationcloud", this is SDK. You can integrate it in your application. It contains both Translation and Storage API
- Module "test", unittests. You can take a look at them to see various code examples.
- Jupyter notebook "demo". Sample demo notebook.

### Dependencies
- See requirements.txt

## Versions support:
- Python :: 2.7
- Python :: 3
- Python :: 3.4
- Python :: 3.5
- Python :: 3.6
- Python :: 3.7
- Python :: 3.8

_________________________

## GroupDocs.Translation Cloud SDKs

||||||||||
|--------------|----------|-------|-------|-------|---------|---------|----------|-------|
|[.NET](https://github.com/groupdocs-translation-cloud/groupdocs-translation-cloud-dotnet)|[Java](https://github.com/groupdocs-translation-cloud/groupdocs-translation-cloud-java)|PHP|Ruby|[Python](https://github.com/groupdocs-translation-cloud/groupdocs-translation-cloud-python)|Node.js|Android|Objective-C|Perl|

[Home](https://www.groupdocs.cloud/) | [Product Page](https://products.groupdocs.cloud/translation/python) | [Docs](https://docs.groupdocs.cloud/translation/) | [Demos](https://products.groupdocs.app/viewer/family) | [API Reference](https://apireference.groupdocs.cloud/translation/) | [Examples](https://github.com/groupdocs-translation-cloud/groupdocs-translation-cloud-python) | [Blog](https://blog.groupdocs.cloud/category/translation/) | [Free Support](https://forum.groupdocs.cloud/c/translation) | [Free Trial](https://purchase.groupdocs.cloud/trial)
