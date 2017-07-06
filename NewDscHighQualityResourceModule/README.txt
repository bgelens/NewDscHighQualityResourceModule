# <%=$PLASTER_PARAM_ModuleName%>

{ Description of the module - Please include any requirements for running all resources in this module (e.g. Must run on Windows Server OS, must have Exchange already installed) - Requirements specific to only certain resources in this module may be listed below with the description of those resources. }

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/)
 or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any
 additional questions or comments.

## Branches

### master

{ appveyor master badge }
{ codecov master badge }

This is the branch containing the latest release - no contributions should be
made directly to this branch.

### dev

{ appveyor dev badge }
{ codecov dev badge }

This is the development branch to which contributions should be proposed by
contributors as pull requests. This development branch will periodically be
merged to the master branch, and be released to [PowerShell Gallery](https://www.powershellgallery.com/).

## Contributing

Please check out common DSC Resources [contributing guidelines](https://github.com/PowerShell/DscResource.Kit/blob/master/CONTRIBUTING.md).

## Resources

* [**<%=$PLASTER_PARAM_ResourceFriendlyName%>**](#<%=$PLASTER_PARAM_ResourceFriendlyName.ToLower()%>) One line description of <%=$PLASTER_PARAM_ResourceFriendlyName%>
* [**Resource2**]() One line description of resource 2}
* ...

### <%=$PLASTER_PARAM_ResourceFriendlyName%>

{ Detailed description of <%=$PLASTER_PARAM_ResourceFriendlyName%> }

#### Requirements for <%=$PLASTER_PARAM_ResourceFriendlyName%>

* { List the requirements for this resource to work (e.g. Role x installed) }

#### Parameters for <%=$PLASTER_PARAM_ResourceFriendlyName%>
<%
    if ($PLASTER_PARAM_Ensure -eq 'Yes') {
        "* **``[String]`` Ensure** _(Write)_: Ensures the resource state. { Present | Absent }."
    }
    if ($PLASTER_PARAM_IsSingleInstance -eq 'Yes') {
        "* **``[String]`` IsSingleInstance** _(Key)_: Specifies the resource is a single instance,"
        " the value must be 'Yes'. { *Yes* }."
    }
%>
* **`[String]` SomeParam** _(Key)_: Description.
 The default value is DefaultValue3. { Value1 | Value2 | *DefaultValue3* }.

#### Read-Only Properties from Get-TargetResource for <%=$PLASTER_PARAM_ResourceFriendlyName%>

{ List any Read-Only Properties here or add the text 'None' if none exist }

#### Examples <%=$PLASTER_PARAM_ResourceFriendlyName%>

* [Example1 description](/Examples/<%=$PLASTER_PARAM_ResourceFriendlyName%>_Example.ps1)
* [Example2 description]()

### Resource2

{ Detailed description of Resource2 }

#### Requirements for Resource2

* { List the requirements for this resource to work (e.g. Role x installed) }

#### Parameters for Resource2

* **`[String]` SomeParam** _(Key)_: Description.
 The default value is DefaultValue3. { Value1 | Value2 | *DefaultValue3* }.

#### Read-Only Properties from Get-TargetResource for Resource2

{ List any Read-Only Properties here or add the text 'None' if none exist }

#### Examples Resource2

* [Example1 description](/Examples/<Resource2_Example.ps1)
* [Example2 description]()

## Versions

### Unreleased

* {Unreleased change 1}
* {Unreleased change 2}
* ...

### <%=$PLASTER_PARAM_Version%>

* Initial release with the following resources:
  * <%=$PLASTER_PARAM_ResourceFriendlyName%>
  * ...