<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [excelnet:autoform Public API](#excelnetautoform-public-api)
  - [<a name="AutoForm.Utility"></a>*AutoForm*.Utility {any}&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformutilityaautoformutility-anynbspnbspsubiclientisub)
  - [<a name="AutoForm.addHooks"></a>*AutoForm*.addHooks(formIds, hooks)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformaddhooksaautoformaddhooksformids-hooksnbspnbspsubiclientisub)
  - [<a name="AutoForm.hooks"></a>*AutoForm*.hooks(hooks)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformhooksaautoformhookshooksnbspnbspsubiclientisub)
  - [<a name="AutoForm._hooks"></a>*AutoForm*._hooks {any}&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoform_hooksaautoform_hooks-anynbspnbspsubiclientisub)
  - [<a name="AutoForm._globalHooks"></a>*AutoForm*._globalHooks {any}&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoform_globalhooksaautoform_globalhooks-anynbspnbspsubiclientisub)
  - [<a name="AutoForm._forceResetFormValues"></a>*AutoForm*._forceResetFormValues(formId)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoform_forceresetformvaluesaautoform_forceresetformvaluesformidnbspnbspsubiclientisub)
  - [<a name="AutoForm.resetForm"></a>*AutoForm*.resetForm(formId, [template])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformresetformaautoformresetformformid-templatenbspnbspsubiclientisub)
  - [<a name="AutoForm.setDefaultTemplate"></a>*AutoForm*.setDefaultTemplate(template)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformsetdefaulttemplateaautoformsetdefaulttemplatetemplatenbspnbspsubiclientisub)
  - [<a name="AutoForm.getDefaultTemplate"></a>*AutoForm*.getDefaultTemplate()&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetdefaulttemplateaautoformgetdefaulttemplatenbspnbspsubiclientisub)
  - [<a name="AutoForm.setDefaultTemplateForType"></a>*AutoForm*.setDefaultTemplateForType(type, template)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformsetdefaulttemplatefortypeaautoformsetdefaulttemplatefortypetype-templatenbspnbspsubiclientisub)
  - [<a name="AutoForm.getDefaultTemplateForType"></a>*AutoForm*.getDefaultTemplateForType(type)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetdefaulttemplatefortypeaautoformgetdefaulttemplatefortypetypenbspnbspsubiclientisub)
  - [<a name="AutoForm.getTemplateName"></a>*AutoForm*.getTemplateName(templateType, templateName, [fieldName], [skipExistsCheck])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgettemplatenameaautoformgettemplatenametemplatetype-templatename-fieldname-skipexistschecknbspnbspsubiclientisub)
  - [<a name="AutoForm.getFormValues"></a>*AutoForm*.getFormValues(formId, [template], [ss], [getModifier])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetformvaluesaautoformgetformvaluesformid-template-ss-getmodifiernbspnbspsubiclientisub)
  - [<a name="AutoForm.getFieldValue"></a>*AutoForm*.getFieldValue(fieldName, [formId])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetfieldvalueaautoformgetfieldvaluefieldname-formidnbspnbspsubiclientisub)
  - [<a name="AutoForm.getInputTypeTemplateNameForElement"></a>*AutoForm*.getInputTypeTemplateNameForElement(element)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetinputtypetemplatenameforelementaautoformgetinputtypetemplatenameforelementelementnbspnbspsubiclientisub)
  - [<a name="AutoForm.getInputValue"></a>*AutoForm*.getInputValue(element, [ss])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetinputvalueaautoformgetinputvalueelement-ssnbspnbspsubiclientisub)
  - [<a name="AutoForm.addInputType"></a>*AutoForm*.addInputType(name, definition)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformaddinputtypeaautoformaddinputtypename-definitionnbspnbspsubiclientisub)
  - [<a name="AutoForm.addFormType"></a>*AutoForm*.addFormType(name, definition)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformaddformtypeaautoformaddformtypename-definitionnbspnbspsubiclientisub)
  - [<a name="AutoForm.validateField"></a>*AutoForm*.validateField(formId, fieldName, [skipEmpty])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformvalidatefieldaautoformvalidatefieldformid-fieldname-skipemptynbspnbspsubiclientisub)
  - [<a name="AutoForm.validateForm"></a>*AutoForm*.validateForm(formId)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformvalidateformaautoformvalidateformformidnbspnbspsubiclientisub)
  - [<a name="AutoForm.getValidationContext"></a>*AutoForm*.getValidationContext([formId])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetvalidationcontextaautoformgetvalidationcontextformidnbspnbspsubiclientisub)
  - [<a name="AutoForm.findAttribute"></a>*AutoForm*.findAttribute(attrName)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformfindattributeaautoformfindattributeattrnamenbspnbspsubiclientisub)
  - [<a name="AutoForm.findAttributesWithPrefix"></a>*AutoForm*.findAttributesWithPrefix(prefix)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformfindattributeswithprefixaautoformfindattributeswithprefixprefixnbspnbspsubiclientisub)
  - [<a name="AutoForm.debug"></a>*AutoForm*.debug()&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformdebugaautoformdebugnbspnbspsubiclientisub)
  - [<a name="AutoForm.arrayTracker"></a>*AutoForm*.arrayTracker {any}&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformarraytrackeraautoformarraytracker-anynbspnbspsubiclientisub)
  - [<a name="AutoForm.getInputType"></a>*AutoForm*.getInputType(atts)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetinputtypeaautoformgetinputtypeattsnbspnbspsubiclientisub)
  - [<a name="AutoForm.getSchemaForField"></a>*AutoForm*.getSchemaForField(name)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetschemaforfieldaautoformgetschemaforfieldnamenbspnbspsubiclientisub)
  - [<a name="AutoForm._getOptionsForField"></a>*AutoForm*._getOptionsForField(name)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoform_getoptionsforfieldaautoform_getoptionsforfieldnamenbspnbspsubiclientisub)
  - [<a name="AutoForm.getLabelForField"></a>*AutoForm*.getLabelForField(name)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetlabelforfieldaautoformgetlabelforfieldnamenbspnbspsubiclientisub)
  - [<a name="AutoForm.templateInstanceForForm"></a>*AutoForm*.templateInstanceForForm([formId])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformtemplateinstanceforformaautoformtemplateinstanceforformformidnbspnbspsubiclientisub)
  - [<a name="AutoForm.viewForForm"></a>*AutoForm*.viewForForm([formId])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformviewforformaautoformviewforformformidnbspnbspsubiclientisub)
  - [<a name="AutoForm.getArrayCountFromDocForField"></a>*AutoForm*.getArrayCountFromDocForField(formId, field)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetarraycountfromdocforfieldaautoformgetarraycountfromdocforfieldformid-fieldnbspnbspsubiclientisub)
  - [<a name="AutoForm.parseData"></a>*AutoForm*.parseData(data)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformparsedataaautoformparsedatadatanbspnbspsubiclientisub)
  - [<a name="AutoForm.getCurrentDataForForm"></a>*AutoForm*.getCurrentDataForForm(formId)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetcurrentdataforformaautoformgetcurrentdataforformformidnbspnbspsubiclientisub)
  - [<a name="AutoForm.getCurrentDataPlusExtrasForForm"></a>*AutoForm*.getCurrentDataPlusExtrasForForm()&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetcurrentdataplusextrasforformaautoformgetcurrentdataplusextrasforformnbspnbspsubiclientisub)
  - [<a name="AutoForm.getFormCollection"></a>*AutoForm*.getFormCollection(formId)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetformcollectionaautoformgetformcollectionformidnbspnbspsubiclientisub)
  - [<a name="AutoForm.getFormSchema"></a>*AutoForm*.getFormSchema([formId], [form])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetformschemaaautoformgetformschemaformid-formnbspnbspsubiclientisub)
  - [<a name="AutoForm.getFormId"></a>*AutoForm*.getFormId()&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformgetformidaautoformgetformidnbspnbspsubiclientisub)
  - [<a name="AutoForm.selectFirstInvalidField"></a>*AutoForm*.selectFirstInvalidField(formId, ss)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformselectfirstinvalidfieldaautoformselectfirstinvalidfieldformid-ssnbspnbspsubiclientisub)
  - [<a name="AutoForm._validateFormDoc"></a>*AutoForm*._validateFormDoc(doc, isModifier, formId, ss, form, [key])&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoform_validateformdocaautoform_validateformdocdoc-ismodifier-formid-ss-form-keynbspnbspsubiclientisub)
  - [<a name="AutoForm.valueConverters.stringToNumber"></a>*AutoFormvalueConverters*.stringToNumber(val)&nbsp;&nbsp;<sub><i>Client</i></sub>](#a-nameautoformvalueconvertersstringtonumberaautoformvalueconvertersstringtonumbervalnbspnbspsubiclientisub)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## excelnet:autoform Public API ##

Easily create forms with automatic insert and update, and automatic reactive validation.

_API documentation automatically generated by [docmeteor](https://github.com/raix/docmeteor)._

-

### <a name="AutoForm.Utility"></a>*AutoForm*.Utility {any}&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This property __Utility__ is defined in `AutoForm`*


> ```AutoForm.Utility = Utility;``` [autoform-api.js:13](autoform-api.js#L13)


-

### <a name="AutoForm.addHooks"></a>*AutoForm*.addHooks(formIds, hooks)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __addHooks__ is defined in `AutoForm`*

__Arguments__

* __formIds__ *{[String[]](#String[])|String|null}*  

 Form `id` or array of form IDs to which these hooks apply. Specify `null` to add hooks that will run for every form.

* __hooks__ *{Object}*  

 Hooks to add, where supported names are "before", "after", "formToDoc", "docToForm", "onSubmit", "onSuccess", and "onError".


__Returns__  *{undefined}*


Defines hooks to be used by one or more forms. Extends hooks lists if called multiple times for the same
form.

> ```AutoForm.addHooks = function autoFormAddHooks(formIds, hooks, replace) { ...``` [autoform-api.js:25](autoform-api.js#L25)


-

### <a name="AutoForm.hooks"></a>*AutoForm*.hooks(hooks)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __hooks__ is defined in `AutoForm`*

__Arguments__

* __hooks__ *{Object}*  

__Returns__  *{undefined}*


Defines hooks by form id. Extends hooks lists if called multiple times for the same
form.

> ```AutoForm.hooks = function autoFormHooks(hooks, replace) { ...``` [autoform-api.js:53](autoform-api.js#L53)


-

### <a name="AutoForm._hooks"></a>*AutoForm*._hooks {any}&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This property ___hooks__ is defined in `AutoForm`*


Hooks list to aid automated testing

> ```AutoForm._hooks = Hooks.form;``` [autoform-api.js:65](autoform-api.js#L65)


-

### <a name="AutoForm._globalHooks"></a>*AutoForm*._globalHooks {any}&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This property ___globalHooks__ is defined in `AutoForm`*


Global hooks list to aid automated testing

> ```AutoForm._globalHooks = Hooks.global;``` [autoform-api.js:73](autoform-api.js#L73)


-

### <a name="AutoForm._forceResetFormValues"></a>*AutoForm*._forceResetFormValues(formId)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method ___forceResetFormValues__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  

__Returns__  *{undefined}*


Forces an AutoForm's values to properly update.
See https:

> ```AutoForm._forceResetFormValues = function autoFormForceResetFormValues(formId) { ...``` [autoform-api.js:84](autoform-api.js#L84)


-

### <a name="AutoForm.resetForm"></a>*AutoForm*.resetForm(formId, [template])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __resetForm__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  
* __template__ *{[TemplateInstance](#TemplateInstance)}*  (Optional)

 Looked up if not provided. Pass in for efficiency.


__Returns__  *{undefined}*


Resets an autoform, including resetting validation errors. The same as clicking the reset button for an autoform.

> ```AutoForm.resetForm = function autoFormResetForm(formId, template) { ...``` [autoform-api.js:102](autoform-api.js#L102)


-

### <a name="AutoForm.setDefaultTemplate"></a>*AutoForm*.setDefaultTemplate(template)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __setDefaultTemplate__ is defined in `AutoForm`*

__Arguments__

* __template__ *{String}*  


> ```AutoForm.setDefaultTemplate = function autoFormSetDefaultTemplate(template) { ...``` [autoform-api.js:113](autoform-api.js#L113)


-

### <a name="AutoForm.getDefaultTemplate"></a>*AutoForm*.getDefaultTemplate()&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getDefaultTemplate__ is defined in `AutoForm`*


Reactive.

> ```AutoForm.getDefaultTemplate = function autoFormGetDefaultTemplate() { ...``` [autoform-api.js:124](autoform-api.js#L124)


-

### <a name="AutoForm.setDefaultTemplateForType"></a>*AutoForm*.setDefaultTemplateForType(type, template)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __setDefaultTemplateForType__ is defined in `AutoForm`*

__Arguments__

* __type__ *{String}*  
* __template__ *{String}*  


> ```AutoForm.setDefaultTemplateForType = function autoFormSetDefaultTemplateForType(type, template) { ...``` [autoform-api.js:135](autoform-api.js#L135)


-

### <a name="AutoForm.getDefaultTemplateForType"></a>*AutoForm*.getDefaultTemplateForType(type)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getDefaultTemplateForType__ is defined in `AutoForm`*

__Arguments__

* __type__ *{String}*  

__Returns__  *{String}*
Template name


Reactive.

> ```AutoForm.getDefaultTemplateForType = function autoFormGetDefaultTemplateForType(type) { ...``` [autoform-api.js:154](autoform-api.js#L154)


-

### <a name="AutoForm.getTemplateName"></a>*AutoForm*.getTemplateName(templateType, templateName, [fieldName], [skipExistsCheck])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getTemplateName__ is defined in `AutoForm`*

__Arguments__

* __templateType__ *{String}*  
* __templateName__ *{String}*  
* __fieldName__ *{String}*  (Optional)
* __skipExistsCheck__ *{Boolean}*  (Optional)

 Pass `true` to return a template name even if that template hasn't been defined.


__Returns__  *{String}*
Template name


Returns the full template name. In the simplest scenario, this is templateType_templateName
as passed in. However, if templateName is not provided, it is looked up in the following
manner:

1. autoform.<componentType>.template from the schema (field+type override for all forms)
2. autoform.template from the schema (field override for all forms)
3. template-<componentType> attribute on an ancestor component within the same form (form+type for all fields)
4. template attribute on an ancestor component within the same form (form specificity for all types and fields)
5. Default template for component type, as set by AutoForm.setDefaultTemplateForType
6. Default template, as set by AutoForm.setDefaultTemplate.
7. Built-in default template, currently bootstrap-3.

> ```AutoForm.getTemplateName = function autoFormGetTemplateName(templateType, templateName, fieldName, skipExistsCheck) { ...``` [autoform-api.js:183](autoform-api.js#L183)


-

### <a name="AutoForm.getFormValues"></a>*AutoForm*.getFormValues(formId, [template], [ss], [getModifier])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getFormValues__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  

 The `id` attribute of the `autoForm` you want current values for.

* __template__ *{[Template](#Template)}*  (Optional)

 The template instance, if already known, as a performance optimization.

* __ss__ *{[SimpleSchema](#SimpleSchema)}*  (Optional)

 The SimpleSchema instance, if already known, as a performance optimization.

* __getModifier__ *{Boolean}*  (Optional)

 Set to `true` to return a modifier object or `false` to return a normal object. For backwards compatibility, and object containing both is returned if this is undefined.


__Returns__  *{Object|null}*


Returns an object representing the current values of all schema-based fields in the form.
The returned object is either a normal object or a MongoDB modifier, based on the `getModifier` argument. Return value may be `null` if the form is not currently rendered on screen.

> ```AutoForm.getFormValues = function autoFormGetFormValues(formId, template, ss, getModifier) { ...``` [autoform-api.js:255](autoform-api.js#L255)


-

### <a name="AutoForm.getFieldValue"></a>*AutoForm*.getFieldValue(fieldName, [formId])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getFieldValue__ is defined in `AutoForm`*

__Arguments__

* __fieldName__ *{String}*  

 The name of the field for which you want the current value.

* __formId__ *{String}*  (Optional)

 The `id` attribute of the `autoForm` you want current values for. Default is the closest form from the current context.


__Returns__  *{Any|undefined}*


Returns the value of the field (the value that would be used if the form were submitted right now).
This is a reactive method that will rerun whenever the current value of the requested field changes. Return value will be undefined if the field is not currently rendered.

> ```AutoForm.getFieldValue = function autoFormGetFieldValue(fieldName, formId) { ...``` [autoform-api.js:411](autoform-api.js#L411)


-

### <a name="AutoForm.getInputTypeTemplateNameForElement"></a>*AutoForm*.getInputTypeTemplateNameForElement(element)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getInputTypeTemplateNameForElement__ is defined in `AutoForm`*

__Arguments__

* __element__ *{[DOMElement](#DOMElement)}*  

 The input DOM element, generated by an autoform input control


__Returns__  *{String}*


Returns the name of the template used to render the element.

> ```AutoForm.getInputTypeTemplateNameForElement = function autoFormGetInputTypeTemplateNameForElement(element) { ...``` [autoform-api.js:446](autoform-api.js#L446)


-

### <a name="AutoForm.getInputValue"></a>*AutoForm*.getInputValue(element, [ss])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getInputValue__ is defined in `AutoForm`*

__Arguments__

* __element__ *{[DOMElement](#DOMElement)}*  

 The input DOM element, generated by an autoform input control, which must have a `data-schema-key` attribute set to the correct schema key name.

* __ss__ *{[SimpleSchema](#SimpleSchema)}*  (Optional)

 Provide the SimpleSchema instance if you already have it.


__Returns__  *{Any}*


Returns the value of the field (the value that would be used if the form were submitted right now).
Unlike `AutoForm.getFieldValue`, this function is not reactive.

> ```AutoForm.getInputValue = function autoFormGetInputValue(element, ss) { ...``` [autoform-api.js:474](autoform-api.js#L474)


-

### <a name="AutoForm.addInputType"></a>*AutoForm*.addInputType(name, definition)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __addInputType__ is defined in `AutoForm`*

__Arguments__

* __name__ *{String}*  

 The type string that this definition is for.

* __definition__ *{Object}*  

 Defines how the input type should be rendered.

    * __componentName__ *{String}*  

    The component name. A template with the name <componentName>_bootstrap3, and potentially others, must be defined.


__Returns__  *{undefined}*


Use this method to add custom input components.

> ```AutoForm.addInputType = function afAddInputType(name, definition) { ...``` [autoform-api.js:541](autoform-api.js#L541)


-

### <a name="AutoForm.addFormType"></a>*AutoForm*.addFormType(name, definition)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __addFormType__ is defined in `AutoForm`*

__Arguments__

* __name__ *{String}*  

 The type string that this definition is for.

* __definition__ *{Object}*  

 Defines how the submit type should work

    * __adjustInputContext__ *{Function}*  (Optional)

    A function that accepts a single argument, which is the context with which an input template in the form will be called, potentially changes the context object, and then returns it. For example, the "readonly" and "disabled" form types use this function to add the "readonly" or "disabled" attribute, respectively, to every input within the form.

    * __adjustSchema__ *{Function}*  (Optional)

    A function that accepts a single argument, which is the form schema, and potentially uses that to return a different schema to use instead. For example, the "update-pushArray" form type uses this function to build and return a schema that is limited by the `scope` attribute on the form. When this function is called, `this` contains useful information about the form.

    * __hideArrayItemButtons__ *{Boolean}*  (Optional)

    Set to `true` if this form type should not show buttons for adding and removing items in an array field. The "disabled" and "readonly" form types do this.

    * __onSubmit__ *{Function}*  

    A function that does whatever should happen upon submission of this form type. When this function is called, `this` contains useful information about the form. At a minimum, you probably want to call `this.event.preventDefault()` to prevent the browser from submitting the form. Your submission logic may want to rely on additional custom form attributes, which will be available in `this.formAttributes`. If you do any additional validation and it fails, you should call `this.failedValidation()`. When your logic is done, you should call `this.result(error, result)`. If you want to end the submission process without providing a result, call `this.endSubmission()`. If you don't call `this.result()` or `this.endSubmission()`, `endSubmit` hooks won't be called, so for example the submit button might remain disabled. `onError` hooks will be called only if you pass an error to `this.result()`. `onSuccess` hooks will be called only if you do not pass an error to `this.result()`.

    * __shouldPrevalidate__ *{Function}*  (Optional)

    A function that returns `true` if validation against the form schema should happen before the `onSubmit` function is called, or `false` if not. When this function is called, `this` contains useful information about the form. If this function is not provided for a form type, the default is `true`.

    * __validateForm__ *{Function}*  

    A function that validates the form and returns `true` if valid or `false` if not. This can happen during submission but also at other times. When this function is called, `this` contains useful information about the form and the validation options.


__Returns__  *{undefined}*


Use this method to add custom form types.

> ```AutoForm.addFormType = function afAddFormType(name, definition) { ...``` [autoform-api.js:562](autoform-api.js#L562)


-

### <a name="AutoForm.validateField"></a>*AutoForm*.validateField(formId, fieldName, [skipEmpty])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __validateField__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  

 The `id` attribute of the `autoForm` you want to validate.

* __fieldName__ *{String}*  

 The name of the field within the `autoForm` you want to validate.

* __skipEmpty__ *{Boolean}*  (Optional, Default = false)

 Set to `true` to skip validation if the field has no value. Useful for preventing `required` errors in form fields that the user has not yet filled out.


__Returns__  *{Boolean}*
Is it valid?


In addition to returning a boolean that indicates whether the field is currently valid,
this method causes the reactive validation messages to appear.

> ```AutoForm.validateField = function autoFormValidateField(formId, fieldName, skipEmpty) { ...``` [autoform-api.js:579](autoform-api.js#L579)


-

### <a name="AutoForm.validateForm"></a>*AutoForm*.validateForm(formId)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __validateForm__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  

 The `id` attribute of the `autoForm` you want to validate.


__Returns__  *{Boolean}*
Is it valid?


In addition to returning a boolean that indicates whether the form is currently valid,
this method causes the reactive validation messages to appear.

> ```AutoForm.validateForm = function autoFormValidateForm(formId) { ...``` [autoform-api.js:592](autoform-api.js#L592)


-

### <a name="AutoForm.getValidationContext"></a>*AutoForm*.getValidationContext([formId])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getValidationContext__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  (Optional)

 The `id` attribute of the `autoForm` for which you want the validation context


__Returns__  *{SimpleSchema.ValidationContext}*
The SimpleSchema validation context object.


Use this method to get the validation context, which can be used to check
the current invalid fields, manually invalidate fields, etc.

> ```AutoForm.getValidationContext = function autoFormGetValidationContext(formId) { ...``` [autoform-api.js:628](autoform-api.js#L628)


-

### <a name="AutoForm.findAttribute"></a>*AutoForm*.findAttribute(attrName)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __findAttribute__ is defined in `AutoForm`*

__Arguments__

* __attrName__ *{String}*  

 Attribute name


__Returns__  *{Any|undefined}*
Searches for the given attribute, looking up the parent context tree until the closest autoform is reached.


Call this method from a UI helper. Might return undefined.

> ```AutoForm.findAttribute = function autoFormFindAttribute(attrName) { ...``` [autoform-api.js:645](autoform-api.js#L645)


-

### <a name="AutoForm.findAttributesWithPrefix"></a>*AutoForm*.findAttributesWithPrefix(prefix)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __findAttributesWithPrefix__ is defined in `AutoForm`*

__Arguments__

* __prefix__ *{String}*  

 Attribute prefix


__Returns__  *{Object}*
An object containing all of the found attributes and their values, with the prefix removed from the keys.


Call this method from a UI helper. Searches for attributes that start with the given prefix, looking up the parent context tree until the closest autoform is reached.

> ```AutoForm.findAttributesWithPrefix = function autoFormFindAttributesWithPrefix(prefix) { ...``` [autoform-api.js:686](autoform-api.js#L686)


-

### <a name="AutoForm.debug"></a>*AutoForm*.debug()&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __debug__ is defined in `AutoForm`*


Call this method in client code while developing to turn on extra logging.
You need to call it just one time, usually in top level client code.

> ```AutoForm.debug = function autoFormDebug() { ...``` [autoform-api.js:730](autoform-api.js#L730)


-

### <a name="AutoForm.arrayTracker"></a>*AutoForm*.arrayTracker {any}&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This property __arrayTracker__ is defined in `AutoForm`*


> ```AutoForm.arrayTracker = arrayTracker;``` [autoform-api.js:743](autoform-api.js#L743)


-

### <a name="AutoForm.getInputType"></a>*AutoForm*.getInputType(atts)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getInputType__ is defined in `AutoForm`*

__Arguments__

* __atts__ *{Object}*  

 The attributes provided to afFieldInput.


__Returns__  *{String}*
The input type. Most are the same as the `type` attributes for HTML input elements, but some are special strings that autoform interprets.


Call this method from a UI helper to get the type string for the input control.

> ```AutoForm.getInputType = function getInputType(atts) { ...``` [autoform-api.js:753](autoform-api.js#L753)


-

### <a name="AutoForm.getSchemaForField"></a>*AutoForm*.getSchemaForField(name)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getSchemaForField__ is defined in `AutoForm`*

__Arguments__

* __name__ *{String}*  

 The field name attribute / schema key.


__Returns__  *{Object|undefined}*


Call this method from a UI helper to get the field definitions based on the schema used by the closest containing autoForm.

> ```AutoForm.getSchemaForField = function autoFormGetSchemaForField(name) { ...``` [autoform-api.js:836](autoform-api.js#L836)


-

### <a name="AutoForm._getOptionsForField"></a>*AutoForm*._getOptionsForField(name)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method ___getOptionsForField__ is defined in `AutoForm`*

__Arguments__

* __name__ *{String}*  

 The field name attribute / schema key.


__Returns__  *{Array(Object)|String|undefined}*


Call this method from a UI helper to get the select options for the field. Might return the string "allowed".

> ```AutoForm._getOptionsForField = function autoFormGetOptionsForField(name) { ...``` [autoform-api.js:850](autoform-api.js#L850)


-

### <a name="AutoForm.getLabelForField"></a>*AutoForm*.getLabelForField(name)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getLabelForField__ is defined in `AutoForm`*

__Arguments__

* __name__ *{String}*  

 The field name attribute / schema key.


__Returns__  *{Object}*


Call this method from a UI helper to get the field definitions based on the schema used by the closest containing autoForm.

> ```AutoForm.getLabelForField = function autoFormGetLabelForField(name) { ...``` [autoform-api.js:884](autoform-api.js#L884)


-

### <a name="AutoForm.templateInstanceForForm"></a>*AutoForm*.templateInstanceForForm([formId])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __templateInstanceForForm__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  (Optional)

 The form's `id` attribute


__Returns__  *{TemplateInstance|undefined}*
The template instance.


Gets the template instance for the form with formId or the closest form to the current context.

> ```AutoForm.templateInstanceForForm = function (formId) { ...``` [autoform-api.js:896](autoform-api.js#L896)


-

### <a name="AutoForm.viewForForm"></a>*AutoForm*.viewForForm([formId])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __viewForForm__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  (Optional)

 The form's `id` attribute. Do not pass this if calling from within a form context.


__Returns__  *{Blaze.View|undefined}*
The `Blaze.View` instance for the autoForm.


Gets the `Blaze.View` instance for the form with formId or the closest form to the current context.

> ```AutoForm.viewForForm = function (formId) { ...``` [autoform-api.js:912](autoform-api.js#L912)


-

### <a name="AutoForm.getArrayCountFromDocForField"></a>*AutoForm*.getArrayCountFromDocForField(formId, field)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getArrayCountFromDocForField__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  

 The form's `id` attribute

* __field__ *{String}*  

 The field name (schema key)


__Returns__  *{Number|undefined}*
Array count in the attached document.


Looks in the document attached to the form to see if the
requested field exists and is an array. If so, returns the
length (count) of the array. Otherwise returns undefined.

> ```AutoForm.getArrayCountFromDocForField = function (formId, field) { ...``` [autoform-api.js:949](autoform-api.js#L949)


-

### <a name="AutoForm.parseData"></a>*AutoForm*.parseData(data)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __parseData__ is defined in `AutoForm`*

__Arguments__

* __data__ *{Object}*  

 Current data context for the form, or an empty object. Usually this is used from a quickForm, since the autoForm won't be rendered yet. Otherwise you should use AutoForm.getCurrentDataForForm if you can.


__Returns__  *{Object}*
Current data context for the form, or an empty object.


Parses and alters the current data context for a form. It will have default values added and a `_resolvedSchema` property that has the schema the form should use.

> ```AutoForm.parseData = function (data) { ...``` [autoform-api.js:969](autoform-api.js#L969)


-

### <a name="AutoForm.getCurrentDataForForm"></a>*AutoForm*.getCurrentDataForForm(formId)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getCurrentDataForForm__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  

 The form's `id` attribute


__Returns__  *{Object}*
Current data context for the form, or an empty object.


Returns the current data context for a form.
You can call this without a formId from within a helper and
the data for the nearest containing form will be returned.

> ```AutoForm.getCurrentDataForForm = function (formId) { ...``` [autoform-api.js:983](autoform-api.js#L983)


-

### <a name="AutoForm.getCurrentDataPlusExtrasForForm"></a>*AutoForm*.getCurrentDataPlusExtrasForForm()&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getCurrentDataPlusExtrasForForm__ is defined in `AutoForm`*

__Arguments__

* ____ *{any}*  

 {String} [formId] The form's `id` attribute


__Returns__  *{Object}*
Current data context for the form, or an empty object.


Returns the current data context for a form plus some extra properties.
You can call this without a formId from within a helper and
the data for the nearest containing form will be returned.

> ```AutoForm.getCurrentDataPlusExtrasForForm = function (formId) { ...``` [autoform-api.js:1005](autoform-api.js#L1005)


-

### <a name="AutoForm.getFormCollection"></a>*AutoForm*.getFormCollection(formId)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getFormCollection__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  

 The form's `id` attribute


__Returns__  *{Mongo.Collection|undefined}*
The Collection instance


Gets the collection for a form from the `collection` attribute

> ```AutoForm.getFormCollection = function (formId) { ...``` [autoform-api.js:1025](autoform-api.js#L1025)


-

### <a name="AutoForm.getFormSchema"></a>*AutoForm*.getFormSchema([formId], [form])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getFormSchema__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  (Optional)

 The form's `id` attribute

* __form__ *{Object}*  (Optional)

 Pass the form data context as an optimization or if the form is not yet rendered.


__Returns__  *{SimpleSchema|undefined}*
The SimpleSchema instance


Gets the schema for a form, from the `schema` attribute if
provided, or from the schema attached to the `Mongo.Collection`
specified in the `collection` attribute. The form must be
currently rendered.

> ```AutoForm.getFormSchema = function (formId, form) { ...``` [autoform-api.js:1042](autoform-api.js#L1042)


-

### <a name="AutoForm.getFormId"></a>*AutoForm*.getFormId()&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __getFormId__ is defined in `AutoForm`*

__Returns__  *{String}*
The containing form's `id` attribute value


Call in a helper to get the containing form's `id` attribute. Reactive.

> ```AutoForm.getFormId = function () { ...``` [autoform-api.js:1054](autoform-api.js#L1054)


-

### <a name="AutoForm.selectFirstInvalidField"></a>*AutoForm*.selectFirstInvalidField(formId, ss)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __selectFirstInvalidField__ is defined in `AutoForm`*

__Arguments__

* __formId__ *{String}*  

 The `id` attribute of the form

* __ss__ *{[SimpleSchema](#SimpleSchema)}*  

 The SimpleSchema instance that was used to create the form's validation context.


__Returns__  *{undefined}*


Selects the focus the first field (in DOM order) with an error.

> ```AutoForm.selectFirstInvalidField = function selectFirstInvalidField(formId, ss) { ...``` [autoform-api.js:1067](autoform-api.js#L1067)


-

### <a name="AutoForm._validateFormDoc"></a>*AutoForm*._validateFormDoc(doc, isModifier, formId, ss, form, [key])&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method ___validateFormDoc__ is defined in `AutoForm`*

__Arguments__

* __doc__ *{Object}*  

 The document with the gathered form values to validate.

* __isModifier__ *{Boolean}*  

 Is `doc` actually a mongo modifier object?

* __formId__ *{String}*  

 The form `id` attribute

* __ss__ *{[SimpleSchema](#SimpleSchema)}*  

 The SimpleSchema instance against which to validate.

* __form__ *{Object}*  

 The form context object

* __key__ *{String}*  (Optional)

 Optionally, a specific schema key to validate.


__Returns__  *{Boolean}*
Is the form valid?


If creating a form type, you will often want to call this from the `validateForm` function. It provides the generic form validation logic that does not typically change between form types.


> ```AutoForm._validateFormDoc = function validateFormDoc(doc, isModifier, formId, ss, form, key) { ...``` [autoform-api.js:1121](autoform-api.js#L1121)


-

### <a name="AutoForm.valueConverters.stringToNumber"></a>*AutoFormvalueConverters*.stringToNumber(val)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __stringToNumber__ is defined in `AutoForm.valueConverters`*

__Arguments__

* __val__ *{String}*  

 A string or null or undefined.


__Returns__  *{Number|String}*
The string converted to a Number or the original value.


For strings, returns Number(val) unless the result is NaN. Otherwise returns val.

> ```stringToNumber: function stringToNumber(val) { ...``` [inputTypes/value-converters.js:141](inputTypes/value-converters.js#L141)


