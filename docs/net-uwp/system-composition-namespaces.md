---
title: "System.Composition namespaces | Microsoft Docs"
ms.custom: ""
ms.date: "12/30/2016"
ms.prod: "windows-client-threshold"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - ".net-for-windows-store-apps"
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 7e857668-26c7-48a0-9aae-011a0cf5b6cb
caps.latest.revision: 10
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
---
# System.Composition namespaces
`System.Composition` and its child namespaces (`System.Composition.Convention`, `System.Composition.Hosting`, and `System.Composition.Hosting.Core`) contain types for developing extensible applications.  
  
 This topic displays the types in the `System.Composition` namespaces that can be installed and used to create [!INCLUDE[win8_appname_long](../net-uwp/includes/win8-appname-long-md.md)] apps.  
  
 To install the following namespaces, open your project in [!INCLUDE[vs_dev11_long](../net-uwp/includes/vs-dev11-long-md.md)] or later, choose **Manage NuGet Packages** from the **Project** menu, and search online for the Microsoft.Composition package.  
  
## System.Composition namespace  
  
|Types supported in the [!INCLUDE[net_win8_profile](../net-uwp/includes/net-win8-profile-md.md)]|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:System.Composition.CompositionContext>|Provides methods to retrieve exports from the composition.|  
|<xref:System.Composition.ExportAttribute>|Specifies that a type, property, field, or method provides a particular export.|  
|<xref:System.Composition.ExportFactory%601>|A factory that creates new instances of a part that provides the specified export.|  
|<xref:System.Composition.ExportFactory%602>|A factory that creates new instances of a part that provides the specified export, with attached metadata.|  
|<xref:System.ComponentModel.Composition.ExportLifetimeContext%601>|Holds an exported value created by an ExportFactory<T\> object and a reference to a method to release that object.|  
|<xref:System.Composition.ExportMetadataAttribute>|Specifies metadata for a type, property, field, or method marked with the ExportAttribute.|  
|<xref:System.Composition.ImportAttribute>|Specifies that a property, field, or parameter value should be provided by the CompositionContainer.object.|  
|<xref:System.Composition.ImportManyAttribute>|Specifies that a property, field, or parameter should be populated with all matching exports by the CompositionContainer object.|  
|<xref:System.Composition.ImportMetadataConstraintAttribute>||  
|<xref:System.Composition.ImportingConstructorAttribute>|Specifies which constructor should be used when creating a part.|  
|<xref:System.Composition.MetadataAttributeAttribute>|Specifies that a custom attribute’s properties provide metadata for exports applied to the same type, property, field, or method.|  
|<xref:System.Composition.OnImportsSatisfiedAttribute>||  
|<xref:System.Composition.PartMetadataAttribute>|Specifies metadata for a part.|  
|<xref:System.Composition.PartNotDiscoverableAttribute>|Specifies that this type’s exports won’t be included in a ComposablePartCatalog.|  
|<xref:System.Composition.SharedAttribute>|Marks the decorated part as being constrained to sharing within the specified boundary.|  
|<xref:System.Composition.SharingBoundaryAttribute>|When applied to an import of an  HYPERLINK "https://msdn.microsoft.com/en-us/library/jj637957(v=vs.110).aspx" ExportFactory<T\> object, marks the boundary of a sharing scope.|  
  
## System.Composition.Convention namespace  
  
|Types supported in the [!INCLUDE[net_win8_profile](../net-uwp/includes/net-win8-profile-md.md)]|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:System.Composition.Convention.AttributedModelProvider>|Provides augmented reflection data to support convention-based models.|  
|<xref:System.Composition.CompositionContextExtensions>||  
|<xref:System.Composition.Convention.ConventionBuilder>|Contains methods to define objects as MEF parts.|  
|<xref:System.Composition.Convention.ExportConventionBuilder>|Configures an export that is associated with a part.|  
|<xref:System.Composition.Convention.ImportConventionBuilder>|Configures an import that is associated with a part.|  
|<xref:System.Composition.Convention.ParameterImportConventionBuilder>|Represents a helper type that is used only in expressions.|  
|<xref:System.Composition.Convention.PartConventionBuilder>|Configures a type as a part.|  
|<xref:System.Composition.Convention.PartConventionBuilder%601>|Configures a type as a part, with strongly typed return values.|  
  
## System.Composition.Hosting namespace  
  
|Types supported in the [!INCLUDE[net_win8_profile](../net-uwp/includes/net-win8-profile-md.md)]|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:System.Composition.Hosting.CompositionFailedException>|The exception that is thrown when composition problems occur.|  
|<xref:System.Composition.Hosting.CompositionHost>|Assembles a lightweight composition container from specified providers.|  
|<xref:System.Composition.Hosting.ContainerConfiguration>|Configures and constructs a lightweight container.|  
  
## System.Composition.Hosting.Core namespace  
  
|Types supported in the [!INCLUDE[net_win8_profile](../net-uwp/includes/net-win8-profile-md.md)]|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:System.Composition.Hosting.Core.CompositeActivator>|The delegate signature that allows instances of parts and exports to be accessed during a composition operation.|  
|<xref:System.Composition.Hosting.Core.CompositionContract>|Defines a standard to match exports and imports.|  
|<xref:System.Composition.Hosting.Core.CompositionDependency>|Describes a dependency that a part must have. Used by the composition engine during initialization to determine whether the composition can be made, and if not, what error to provide.|  
|<xref:System.Composition.Hosting.Core.CompositionOperation>|Represents a single composition operation.|  
|<xref:System.Composition.Hosting.Core.DependencyAccessor>|Allows export providers to locate their dependencies.|  
|<xref:System.Composition.Hosting.Core.ExportDescriptor>|Describes an export of a part known to the composition engine.|  
|<xref:System.Composition.Hosting.Core.ExportDescriptorPromise>|Represents an export descriptor that an available part can provide.|  
|<xref:System.Composition.Hosting.Core.ExportDescriptorProvider>|An object that contributes to the composition.|  
|<xref:System.Composition.Hosting.Core.LifetimeContext>|Represents a node in the lifetime tree.|  
  
## See Also  
 [.NET for Windows apps](../net-uwp/dotnet-for-windows-apps.md)