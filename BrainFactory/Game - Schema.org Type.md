[Schema.org](/)

[![menu](https://schema.org/Game/docs/menu-bar-icon-white.png)](javascript:void(0);)

- [Docs](/docs/documents.html)
- [Schemas](/docs/schemas.html)
- [Validate](https://validator.schema.org)
- [About](/docs/about.html)

|   |   |   |
|---|---|---|
|\|   \|   \|<br>\|---\|---\|<br>\|[×](javascript:void(0) "Clear search box")\||||

**Note**: you are viewing the development version of [Schema.org](https://schema.org). See [How we work](/docs/howwework.html) for more details.

# Game

_A Schema.org Type_  

[Thing](/Thing "Thing") > [CreativeWork](/CreativeWork "CreativeWork") > [Game](/Game "Game")  

**[more...]**

- Canonical URL: https://schema.org/Game
- [Check for open issues.](https://github.com/schemaorg/schemaorg/issues?q=is%3Aissue+is%3Aopen+Game)

The Game type represents things which are games. These are typically rule-governed recreational activities, e.g. role-playing games in which players assume the role of characters in a fictional setting.

|Property|Expected Type|Description|
|---|---|---|
|Properties from [Game](/Game "Game")|   |   |
|`[characterAttribute](/characterAttribute "characterAttribute")`|[Thing](/Thing "Thing")|A piece of data that represents a particular aspect of a fictional character (skill, power, character points, advantage, disadvantage).|
|`[gameItem](/gameItem "gameItem")`|[Thing](/Thing "Thing")|An item is an object within the game world that can be collected by a player or, occasionally, a non-player character.|
|`[gameLocation](/gameLocation "gameLocation")`|[Place](/Place "Place")  or  <br>[PostalAddress](/PostalAddress "PostalAddress")  or  <br>[URL](/URL "URL")|Real or fictional location of the game (or part of game).|
|`[numberOfPlayers](/numberOfPlayers "numberOfPlayers")`|[QuantitativeValue](/QuantitativeValue "QuantitativeValue")|Indicate how many people can play this game (minimum, maximum, or range).|
|`[quest](/quest "quest")`|[Thing](/Thing "Thing")|The task that a player-controlled character, or group of characters may complete in order to gain a reward.|
|Properties from [CreativeWork](/CreativeWork "CreativeWork")|   |   |
|`[about](/about "about")`|[Thing](/Thing "Thing")|The subject matter of the content.  <br>Inverse property: [subjectOf](/subjectOf "subjectOf")|
|`[abstract](/abstract "abstract")`|[Text](/Text "Text")|An abstract is a short description that summarizes a [CreativeWork](/CreativeWork).|
|`[accessMode](/accessMode "accessMode")`|[Text](/Text "Text")|The human sensory perceptual system or cognitive faculty through which a person may process or perceive information. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessMode-vocabulary).|
|`[accessModeSufficient](/accessModeSufficient "accessModeSufficient")`|[ItemList](/ItemList "ItemList")|A list of single or combined accessModes that are sufficient to understand all the intellectual content of a resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessModeSufficient-vocabulary).|
|`[accessibilityAPI](/accessibilityAPI "accessibilityAPI")`|[Text](/Text "Text")|Indicates that the resource is compatible with the referenced accessibility API. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityAPI-vocabulary).|
|`[accessibilityControl](/accessibilityControl "accessibilityControl")`|[Text](/Text "Text")|Identifies input methods that are sufficient to fully control the described resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityControl-vocabulary).|
|`[accessibilityFeature](/accessibilityFeature "accessibilityFeature")`|[Text](/Text "Text")|Content features of the resource, such as accessible media, alternatives and supported enhancements for accessibility. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityFeature-vocabulary).|
|`[accessibilityHazard](/accessibilityHazard "accessibilityHazard")`|[Text](/Text "Text")|A characteristic of the described resource that is physiologically dangerous to some users. Related to WCAG 2.0 guideline 2.3. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityHazard-vocabulary).|
|`[accessibilitySummary](/accessibilitySummary "accessibilitySummary")`|[Text](/Text "Text")|A human-readable summary of specific accessibility features or deficiencies, consistent with the other accessibility metadata but expressing subtleties such as "short descriptions are present but long descriptions will be needed for non-visual users" or "short descriptions are present and no long descriptions are needed".|
|`[accountablePerson](/accountablePerson "accountablePerson")`|[Person](/Person "Person")|Specifies the Person that is legally accountable for the CreativeWork.|
|`[acquireLicensePage](/acquireLicensePage "acquireLicensePage")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL")|Indicates a page documenting how licenses can be purchased or otherwise acquired, for the current item.|
|`[aggregateRating](/aggregateRating "aggregateRating")`|[AggregateRating](/AggregateRating "AggregateRating")|The overall rating, based on a collection of reviews or ratings, of the item.|
|`[alternativeHeadline](/alternativeHeadline "alternativeHeadline")`|[Text](/Text "Text")|A secondary title of the CreativeWork.|
|`[archivedAt](/archivedAt "archivedAt")`|[URL](/URL "URL")  or  <br>[WebPage](/WebPage "WebPage")|Indicates a page or other link involved in archival of a [CreativeWork](/CreativeWork). In the case of [MediaReview](/MediaReview), the items in a [MediaReviewItem](/MediaReviewItem) may often become inaccessible, but be archived by archival, journalistic, activist, or law enforcement organizations. In such cases, the referenced page may not directly publish the content.|
|`[assesses](/assesses "assesses")`|[DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")|The item being described is intended to assess the competency or learning outcome defined by the referenced term.|
|`[associatedMedia](/associatedMedia "associatedMedia")`|[MediaObject](/MediaObject "MediaObject")|A media object that encodes this CreativeWork. This property is a synonym for encoding.|
|`[audience](/audience "audience")`|[Audience](/Audience "Audience")|An intended audience, i.e. a group for whom something was created. Supersedes [serviceAudience](/serviceAudience "serviceAudience").|
|`[audio](/audio "audio")`|[AudioObject](/AudioObject "AudioObject")  or  <br>[Clip](/Clip "Clip")  or  <br>[MusicRecording](/MusicRecording "MusicRecording")|An embedded audio object.|
|`[author](/author "author")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably.|
|`[award](/award "award")`|[Text](/Text "Text")|An award won by or for this item. Supersedes [awards](/awards "awards").|
|`[character](/character "character")`|[Person](/Person "Person")|Fictional person connected with a creative work.|
|`[citation](/citation "citation")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Text](/Text "Text")|A citation or reference to another creative work, such as another publication, web page, scholarly article, etc.|
|`[comment](/comment "comment")`|[Comment](/Comment "Comment")|Comments, typically from users.|
|`[commentCount](/commentCount "commentCount")`|[Integer](/Integer "Integer")|The number of comments this CreativeWork (e.g. Article, Question or Answer) has received. This is most applicable to works published in Web sites with commenting system; additional comments may exist elsewhere.|
|`[conditionsOfAccess](/conditionsOfAccess "conditionsOfAccess")`|[Text](/Text "Text")|Conditions that affect the availability of, or method(s) of access to, an item. Typically used for real world items such as an [ArchiveComponent](/ArchiveComponent) held by an [ArchiveOrganization](/ArchiveOrganization). This property is not suitable for use as a general Web access control mechanism. It is expressed only in natural language.  <br>  <br>For example "Available by appointment from the Reading Room" or "Accessible only from logged-in accounts ".|
|`[contentLocation](/contentLocation "contentLocation")`|[Place](/Place "Place")|The location depicted or described in the content. For example, the location in a photograph or painting.|
|`[contentRating](/contentRating "contentRating")`|[Rating](/Rating "Rating")  or  <br>[Text](/Text "Text")|Official rating of a piece of content—for example, 'MPAA PG-13'.|
|`[contentReferenceTime](/contentReferenceTime "contentReferenceTime")`|[DateTime](/DateTime "DateTime")|The specific time described by a creative work, for works (e.g. articles, video objects etc.) that emphasise a particular moment within an Event.|
|`[contributor](/contributor "contributor")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|A secondary contributor to the CreativeWork or Event.|
|`[copyrightHolder](/copyrightHolder "copyrightHolder")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|The party holding the legal copyright to the CreativeWork.|
|`[copyrightNotice](/copyrightNotice "copyrightNotice")`|[Text](/Text "Text")|Text of a notice appropriate for describing the copyright aspects of this Creative Work, ideally indicating the owner of the copyright for the Work.|
|`[copyrightYear](/copyrightYear "copyrightYear")`|[Number](/Number "Number")|The year during which the claimed copyright for the CreativeWork was first asserted.|
|`[correction](/correction "correction")`|[CorrectionComment](/CorrectionComment "CorrectionComment")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL")|Indicates a correction to a [CreativeWork](/CreativeWork), either via a [CorrectionComment](/CorrectionComment), textually or in another document.|
|`[countryOfOrigin](/countryOfOrigin "countryOfOrigin")`|[Country](/Country "Country")|The country of origin of something, including products as well as creative works such as movie and TV content.  <br>  <br>In the case of TV and movie, this would be the country of the principle offices of the production company or individual responsible for the movie. For other kinds of [CreativeWork](/CreativeWork) it is difficult to provide fully general guidance, and properties such as [contentLocation](/contentLocation) and [locationCreated](/locationCreated) may be more applicable.  <br>  <br>In the case of products, the country of origin of the product. The exact interpretation of this may vary by context and product type, and cannot be fully enumerated here.|
|`[creativeWorkStatus](/creativeWorkStatus "creativeWorkStatus")`|[DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")|The status of a creative work in terms of its stage in a lifecycle. Example terms include Incomplete, Draft, Published, Obsolete. Some organizations define a set of terms for the stages of their publication lifecycle.|
|`[creator](/creator "creator")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.|
|`[creditText](/creditText "creditText")`|[Text](/Text "Text")|Text that can be used to credit person(s) and/or organization(s) associated with a published Creative Work.|
|`[dateCreated](/dateCreated "dateCreated")`|[Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime")|The date on which the CreativeWork was created or the item was added to a DataFeed.|
|`[dateModified](/dateModified "dateModified")`|[Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime")|The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.|
|`[datePublished](/datePublished "datePublished")`|[Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime")|Date of first publication or broadcast. For example the date a [CreativeWork](/CreativeWork) was broadcast or a [Certification](/Certification) was issued.|
|`[digitalSourceType](/digitalSourceType "digitalSourceType")`|[IPTCDigitalSourceEnumeration](/IPTCDigitalSourceEnumeration "IPTCDigitalSourceEnumeration")|Indicates an IPTCDigitalSourceEnumeration code indicating the nature of the digital source(s) for some [CreativeWork](/CreativeWork).|
|`[discussionUrl](/discussionUrl "discussionUrl")`|[URL](/URL "URL")|A link to the page containing the comments of the CreativeWork.|
|`[editEIDR](/editEIDR "editEIDR")`|[Text](/Text "Text")  or  <br>[URL](/URL "URL")|An [EIDR](https://eidr.org/) (Entertainment Identifier Registry) [identifier](/identifier) representing a specific edit / edition for a work of film or television.  <br>  <br>For example, the motion picture known as "Ghostbusters" whose [titleEIDR](/titleEIDR) is "10.5240/7EC7-228A-510A-053E-CBB8-J" has several edits, e.g. "10.5240/1F2A-E1C5-680A-14C6-E76B-I" and "10.5240/8A35-3BEE-6497-5D12-9E4F-3".  <br>  <br>Since schema.org types like [Movie](/Movie) and [TVEpisode](/TVEpisode) can be used for both works and their multiple expressions, it is possible to use [titleEIDR](/titleEIDR) alone (for a general description), or alongside [editEIDR](/editEIDR) for a more edit-specific description.|
|`[editor](/editor "editor")`|[Person](/Person "Person")|Specifies the Person who edited the CreativeWork.|
|`[educationalAlignment](/educationalAlignment "educationalAlignment")`|[AlignmentObject](/AlignmentObject "AlignmentObject")|An alignment to an established educational framework.  <br>  <br>This property should not be used where the nature of the alignment can be described using a simple property, for example to express that a resource [teaches](/teaches) or [assesses](/assesses) a competency.|
|`[educationalLevel](/educationalLevel "educationalLevel")`|[DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL")|The level in terms of progression through an educational or training context. Examples of educational levels include 'beginner', 'intermediate' or 'advanced', and formal sets of level indicators.|
|`[educationalUse](/educationalUse "educationalUse")`|[DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")|The purpose of a work in the context of education; for example, 'assignment', 'group work'.|
|`[encoding](/encoding "encoding")`|[MediaObject](/MediaObject "MediaObject")|A media object that encodes this CreativeWork. This property is a synonym for associatedMedia. Supersedes [encodings](/encodings "encodings").  <br>Inverse property: [encodesCreativeWork](/encodesCreativeWork "encodesCreativeWork")|
|`[encodingFormat](/encodingFormat "encodingFormat")`|[Text](/Text "Text")  or  <br>[URL](/URL "URL")|Media type typically expressed using a MIME format (see [IANA site](http://www.iana.org/assignments/media-types/media-types.xhtml) and [MDN reference](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)), e.g. application/zip for a SoftwareApplication binary, audio/mpeg for .mp3 etc.  <br>  <br>In cases where a [CreativeWork](/CreativeWork) has several media type representations, [encoding](/encoding) can be used to indicate each [MediaObject](/MediaObject) alongside particular [encodingFormat](/encodingFormat) information.  <br>  <br>Unregistered or niche encoding and file formats can be indicated instead via the most appropriate URL, e.g. defining Web page or a Wikipedia/Wikidata entry. Supersedes [fileFormat](/fileFormat "fileFormat").|
|`[exampleOfWork](/exampleOfWork "exampleOfWork")`|[CreativeWork](/CreativeWork "CreativeWork")|A creative work that this work is an example/instance/realization/derivation of.  <br>Inverse property: [workExample](/workExample "workExample")|
|`[expires](/expires "expires")`|[Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime")|Date the content expires and is no longer useful or available. For example a [VideoObject](/VideoObject) or [NewsArticle](/NewsArticle) whose availability or relevance is time-limited, a [ClaimReview](/ClaimReview) fact check whose publisher wants to indicate that it may no longer be relevant (or helpful to highlight) after some date, or a [Certification](/Certification) the validity has expired.|
|`[funder](/funder "funder")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|A person or organization that supports (sponsors) something through some kind of financial contribution.|
|`[funding](/funding "funding")`|[Grant](/Grant "Grant")|A [Grant](/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](/ownershipFundingInfo).  <br>Inverse property: [fundedItem](/fundedItem "fundedItem")|
|`[genre](/genre "genre")`|[Text](/Text "Text")  or  <br>[URL](/URL "URL")|Genre of the creative work, broadcast channel or group.|
|`[hasPart](/hasPart "hasPart")`|[CreativeWork](/CreativeWork "CreativeWork")|Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).  <br>Inverse property: [isPartOf](/isPartOf "isPartOf")|
|`[headline](/headline "headline")`|[Text](/Text "Text")|Headline of the article.|
|`[inLanguage](/inLanguage "inLanguage")`|[Language](/Language "Language")  or  <br>[Text](/Text "Text")|The language of the content or performance or used in an action. Please use one of the language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). See also [availableLanguage](/availableLanguage). Supersedes [language](/language "language").|
|`[interactionStatistic](/interactionStatistic "interactionStatistic")`|[InteractionCounter](/InteractionCounter "InteractionCounter")|The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes [interactionCount](/interactionCount "interactionCount").|
|`[interactivityType](/interactivityType "interactivityType")`|[Text](/Text "Text")|The predominant mode of learning supported by the learning resource. Acceptable values are 'active', 'expositive', or 'mixed'.|
|`[interpretedAsClaim](/interpretedAsClaim "interpretedAsClaim")`|[Claim](/Claim "Claim")|Used to indicate a specific claim contained, implied, translated or refined from the content of a [MediaObject](/MediaObject) or other [CreativeWork](/CreativeWork). The interpreting party can be indicated using [claimInterpreter](/claimInterpreter).|
|`[isAccessibleForFree](/isAccessibleForFree "isAccessibleForFree")`|[Boolean](/Boolean "Boolean")|A flag to signal that the item, event, or place is accessible for free. Supersedes [free](/free "free").|
|`[isBasedOn](/isBasedOn "isBasedOn")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Product](/Product "Product")  or  <br>[URL](/URL "URL")|A resource from which this work is derived or from which it is a modification or adaptation. Supersedes [isBasedOnUrl](/isBasedOnUrl "isBasedOnUrl").|
|`[isFamilyFriendly](/isFamilyFriendly "isFamilyFriendly")`|[Boolean](/Boolean "Boolean")|Indicates whether this content is family friendly.|
|`[isPartOf](/isPartOf "isPartOf")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL")|Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.  <br>Inverse property: [hasPart](/hasPart "hasPart")|
|`[keywords](/keywords "keywords")`|[DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL")|Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property.|
|`[learningResourceType](/learningResourceType "learningResourceType")`|[DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")|The predominant type or kind characterizing the learning resource. For example, 'presentation', 'handout'.|
|`[license](/license "license")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL")|A license document that applies to this content, typically indicated by URL.|
|`[locationCreated](/locationCreated "locationCreated")`|[Place](/Place "Place")|The location where the CreativeWork was created, which may not be the same as the location depicted in the CreativeWork.|
|`[mainEntity](/mainEntity "mainEntity")`|[Thing](/Thing "Thing")|Indicates the primary entity described in some page or other CreativeWork.  <br>Inverse property: [mainEntityOfPage](/mainEntityOfPage "mainEntityOfPage")|
|`[maintainer](/maintainer "maintainer")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|A maintainer of a [Dataset](/Dataset), software package ([SoftwareApplication](/SoftwareApplication)), or other [Project](/Project). A maintainer is a [Person](/Person) or [Organization](/Organization) that manages contributions to, and/or publication of, some (typically complex) artifact. It is common for distributions of software and data to be based on "upstream" sources. When [maintainer](/maintainer) is applied to a specific version of something e.g. a particular version or packaging of a [Dataset](/Dataset), it is always possible that the upstream source has a different maintainer. The [isBasedOn](/isBasedOn) property can be used to indicate such relationships between datasets to make the different maintenance roles clear. Similarly in the case of software, a package may have dedicated maintainers working on integration into software distributions such as Ubuntu, as well as upstream maintainers of the underlying work.|
|`[material](/material "material")`|[Product](/Product "Product")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL")|A material that something is made from, e.g. leather, wool, cotton, paper.|
|`[materialExtent](/materialExtent "materialExtent")`|[QuantitativeValue](/QuantitativeValue "QuantitativeValue")  or  <br>[Text](/Text "Text")|The quantity of the materials being described or an expression of the physical space they occupy.|
|`[mentions](/mentions "mentions")`|[Thing](/Thing "Thing")|Indicates that the CreativeWork contains a reference to, but is not necessarily about a concept.|
|`[offers](/offers "offers")`|[Demand](/Demand "Demand")  or  <br>[Offer](/Offer "Offer")|An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer.  <br>Inverse property: [itemOffered](/itemOffered "itemOffered")|
|`[pattern](/pattern "pattern")`|[DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")|A pattern that something has, for example 'polka dot', 'striped', 'Canadian flag'. Values are typically expressed as text, although links to controlled value schemes are also supported.|
|`[position](/position "position")`|[Integer](/Integer "Integer")  or  <br>[Text](/Text "Text")|The position of an item in a series or sequence of items.|
|`[producer](/producer "producer")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|The person or organization who produced the work (e.g. music album, movie, TV/radio series etc.).|
|`[provider](/provider "provider")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|The service provider, service operator, or service performer; the goods producer. Another party (a seller) may offer those services or goods on behalf of the provider. A provider may also serve as the seller. Supersedes [carrier](/carrier "carrier").|
|`[publication](/publication "publication")`|[PublicationEvent](/PublicationEvent "PublicationEvent")|A publication event associated with the item.|
|`[publisher](/publisher "publisher")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|The publisher of the creative work.|
|`[publisherImprint](/publisherImprint "publisherImprint")`|[Organization](/Organization "Organization")|The publishing division which published the comic.|
|`[publishingPrinciples](/publishingPrinciples "publishingPrinciples")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL")|The publishingPrinciples property indicates (typically via [URL](/URL)) a document describing the editorial principles of an [Organization](/Organization) (or individual, e.g. a [Person](/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](/CreativeWork) (e.g. [NewsArticle](/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](/CreativeWork).  <br>  <br>While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](/funder)) can be expressed using schema.org terminology.|
|`[recordedAt](/recordedAt "recordedAt")`|[Event](/Event "Event")|The Event where the CreativeWork was recorded. The CreativeWork may capture all or part of the event.  <br>Inverse property: [recordedIn](/recordedIn "recordedIn")|
|`[releasedEvent](/releasedEvent "releasedEvent")`|[PublicationEvent](/PublicationEvent "PublicationEvent")|The place and time the release was issued, expressed as a PublicationEvent.|
|`[review](/review "review")`|[Review](/Review "Review")|A review of the item. Supersedes [reviews](/reviews "reviews").|
|`[schemaVersion](/schemaVersion "schemaVersion")`|[Text](/Text "Text")  or  <br>[URL](/URL "URL")|Indicates (by URL or string) a particular version of a schema used in some CreativeWork. This property was created primarily to indicate the use of a specific schema.org release, e.g. `10.0` as a simple string, or more explicitly via URL, `https://schema.org/docs/releases.html#v10.0`. There may be situations in which other schemas might usefully be referenced this way, e.g. `http://dublincore.org/specifications/dublin-core/dces/1999-07-02/` but this has not been carefully explored in the community.|
|`[sdDatePublished](/sdDatePublished "sdDatePublished")`|[Date](/Date "Date")|Indicates the date on which the current structured data was generated / published. Typically used alongside [sdPublisher](/sdPublisher).|
|`[sdLicense](/sdLicense "sdLicense")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL")|A license document that applies to this structured data, typically indicated by URL.|
|`[sdPublisher](/sdPublisher "sdPublisher")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|Indicates the party responsible for generating and publishing the current structured data markup, typically in cases where the structured data is derived automatically from existing published content but published on a different site. For example, student projects and open data initiatives often re-publish existing content with more explicitly structured metadata. The [sdPublisher](/sdPublisher) property helps make such practices more explicit.|
|`[size](/size "size")`|[DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[QuantitativeValue](/QuantitativeValue "QuantitativeValue")  or  <br>[SizeSpecification](/SizeSpecification "SizeSpecification")  or  <br>[Text](/Text "Text")|A standardized size of a product or creative work, specified either through a simple textual string (for example 'XL', '32Wx34L'), a QuantitativeValue with a unitCode, or a comprehensive and structured [SizeSpecification](/SizeSpecification); in other cases, the [width](/width), [height](/height), [depth](/depth) and [weight](/weight) properties may be more applicable.|
|`[sourceOrganization](/sourceOrganization "sourceOrganization")`|[Organization](/Organization "Organization")|The Organization on whose behalf the creator was working.|
|`[spatial](/spatial "spatial")`|[Place](/Place "Place")|The "spatial" property can be used in cases when more specific properties (e.g. [locationCreated](/locationCreated), [spatialCoverage](/spatialCoverage), [contentLocation](/contentLocation)) are not known to be appropriate.|
|`[spatialCoverage](/spatialCoverage "spatialCoverage")`|[Place](/Place "Place")|The spatialCoverage of a CreativeWork indicates the place(s) which are the focus of the content. It is a subproperty of contentLocation intended primarily for more technical and detailed materials. For example with a Dataset, it indicates areas that the dataset describes: a dataset of New York weather would have spatialCoverage which was the place: the state of New York.|
|`[sponsor](/sponsor "sponsor")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event.|
|`[teaches](/teaches "teaches")`|[DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")|The item being described is intended to help a person learn the competency or learning outcome defined by the referenced term.|
|`[temporal](/temporal "temporal")`|[DateTime](/DateTime "DateTime")  or  <br>[Text](/Text "Text")|The "temporal" property can be used in cases where more specific properties (e.g. [temporalCoverage](/temporalCoverage), [dateCreated](/dateCreated), [dateModified](/dateModified), [datePublished](/datePublished)) are not known to be appropriate.|
|`[temporalCoverage](/temporalCoverage "temporalCoverage")`|[DateTime](/DateTime "DateTime")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL")|The temporalCoverage of a CreativeWork indicates the period that the content applies to, i.e. that it describes, either as a DateTime or as a textual string indicating a time period in [ISO 8601 time interval format](https://en.wikipedia.org/wiki/ISO_8601#Time_intervals). In the case of a Dataset it will typically indicate the relevant time period in a precise notation (e.g. for a 2011 census dataset, the year 2011 would be written "2011/2012"). Other forms of content, e.g. ScholarlyArticle, Book, TVSeries or TVEpisode, may indicate their temporalCoverage in broader terms - textually or via well-known URL. Written works such as books may sometimes have precise temporal coverage too, e.g. a work set in 1939 - 1945 can be indicated in ISO 8601 interval format format via "1939/1945".  <br>  <br>Open-ended date ranges can be written with ".." in place of the end date. For example, "2015-11/.." indicates a range beginning in November 2015 and with no specified final date. This is tentative and might be updated in future when ISO 8601 is officially updated. Supersedes [datasetTimeInterval](/datasetTimeInterval "datasetTimeInterval").|
|`[text](/text "text")`|[Text](/Text "Text")|The textual content of this CreativeWork.|
|`[thumbnail](/thumbnail "thumbnail")`|[ImageObject](/ImageObject "ImageObject")|Thumbnail image for an image or video.|
|`[thumbnailUrl](/thumbnailUrl "thumbnailUrl")`|[URL](/URL "URL")|A thumbnail image relevant to the Thing.|
|`[timeRequired](/timeRequired "timeRequired")`|[Duration](/Duration "Duration")|Approximate or typical time it usually takes to work with or through the content of this work for the typical or target audience.|
|`[translationOfWork](/translationOfWork "translationOfWork")`|[CreativeWork](/CreativeWork "CreativeWork")|The work that this work has been translated from. E.g. 物种起源 is a translationOf “On the Origin of Species”.  <br>Inverse property: [workTranslation](/workTranslation "workTranslation")|
|`[translator](/translator "translator")`|[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person")|Organization or person who adapts a creative work to different languages, regional differences and technical requirements of a target market, or that translates during some event.|
|`[typicalAgeRange](/typicalAgeRange "typicalAgeRange")`|[Text](/Text "Text")|The typical expected age range, e.g. '7-9', '11-'.|
|`[usageInfo](/usageInfo "usageInfo")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL")|The schema.org [usageInfo](/usageInfo) property indicates further information about a [CreativeWork](/CreativeWork). This property is applicable both to works that are freely available and to those that require payment or other transactions. It can reference additional information, e.g. community expectations on preferred linking and citation conventions, as well as purchasing details. For something that can be commercially licensed, usageInfo can provide detailed, resource-specific information about licensing options.  <br>  <br>This property can be used alongside the license property which indicates license(s) applicable to some piece of content. The usageInfo property can provide information about other licensing options, e.g. acquiring commercial usage rights for an image that is also available under non-commercial creative commons licenses.|
|`[version](/version "version")`|[Number](/Number "Number")  or  <br>[Text](/Text "Text")|The version of the CreativeWork embodied by a specified resource.|
|`[video](/video "video")`|[Clip](/Clip "Clip")  or  <br>[VideoObject](/VideoObject "VideoObject")|An embedded video object.|
|`[workExample](/workExample "workExample")`|[CreativeWork](/CreativeWork "CreativeWork")|Example/instance/realization/derivation of the concept of this creative work. E.g. the paperback edition, first edition, or e-book.  <br>Inverse property: [exampleOfWork](/exampleOfWork "exampleOfWork")|
|`[workTranslation](/workTranslation "workTranslation")`|[CreativeWork](/CreativeWork "CreativeWork")|A work that is a translation of the content of this work. E.g. 西遊記 has an English workTranslation “Journey to the West”, a German workTranslation “Monkeys Pilgerfahrt” and a Vietnamese translation Tây du ký bình khảo.  <br>Inverse property: [translationOfWork](/translationOfWork "translationOfWork")|
|Properties from [Thing](/Thing "Thing")|   |   |
|`[additionalType](/additionalType "additionalType")`|[Text](/Text "Text")  or  <br>[URL](/URL "URL")|An additional type for the item, typically used for adding more specific types from external vocabularies in microdata syntax. This is a relationship between something and a class that the thing is in. Typically the value is a URI-identified RDF class, and in this case corresponds to the use of rdf:type in RDF. Text values can be used sparingly, for cases where useful information can be added without their being an appropriate schema to reference. In the case of text values, the class label should follow the schema.org [style guide](https://schema.org/docs/styleguide.html).|
|`[alternateName](/alternateName "alternateName")`|[Text](/Text "Text")|An alias for the item.|
|`[description](/description "description")`|[Text](/Text "Text")  or  <br>[TextObject](/TextObject "TextObject")|A description of the item.|
|`[disambiguatingDescription](/disambiguatingDescription "disambiguatingDescription")`|[Text](/Text "Text")|A sub property of description. A short description of the item used to disambiguate from other, similar items. Information from other properties (in particular, name) may be necessary for the description to be useful for disambiguation.|
|`[identifier](/identifier "identifier")`|[PropertyValue](/PropertyValue "PropertyValue")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL")|The identifier property represents any kind of identifier for any kind of [Thing](/Thing), such as ISBNs, GTIN codes, UUIDs etc. Schema.org provides dedicated properties for representing many of these, either as textual strings or as URL (URI) links. See [background notes](/docs/datamodel.html#identifierBg) for more details.|
|`[image](/image "image")`|[ImageObject](/ImageObject "ImageObject")  or  <br>[URL](/URL "URL")|An image of the item. This can be a [URL](/URL) or a fully described [ImageObject](/ImageObject).|
|`[mainEntityOfPage](/mainEntityOfPage "mainEntityOfPage")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL")|Indicates a page (or other CreativeWork) for which this thing is the main entity being described. See [background notes](/docs/datamodel.html#mainEntityBackground) for details.  <br>Inverse property: [mainEntity](/mainEntity "mainEntity")|
|`[name](/name "name")`|[Text](/Text "Text")|The name of the item.|
|`[potentialAction](/potentialAction "potentialAction")`|[Action](/Action "Action")|Indicates a potential Action, which describes an idealized action in which this thing would play an 'object' role.|
|`[sameAs](/sameAs "sameAs")`|[URL](/URL "URL")|URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.|
|`[subjectOf](/subjectOf "subjectOf")`|[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Event](/Event "Event")|A CreativeWork or Event about this Thing.  <br>Inverse property: [about](/about "about")|
|`[url](/url "url")`|[URL](/URL "URL")|URL of the item.|

  

#### More specific Types

- [VideoGame](/VideoGame "VideoGame")

#### [Examples](#examples "Link: #examples")

[Example 1](#eg-0452 "Link: #eg-0452")

 ![Copy to clipboard](https://schema.org/Game/docs/clipboard/clippy.svg)Copied

No Markup Microdata RDFa JSON-LD Structure

Example notes or example HTML without markup.

1. <section>  
    
2.     <section>  
    
3.       <span>Approx. Retail:</span>  
    
4.       <span>$17.99</span>  
    
5.       <a href="/monopoly-2/en_US/shop/where-to-buy.cfm?brand_guid=DAD28866-1C43-11DD-BD0B-0800200C9A66&prodName=Monopoly%20Game">Where To Buy</a>  
    
6.     </section>  
    
7.     <span>  
    
8.       Ages: <span>8</span> YEARS &amp; UP  
    
9.     </span>  
    
10.     <h4>Game Description:</h4>  
    
11.     <p>Own it all as a high-flying trader in the fast-paced world of real estate. Tour the city for the hottest properties: sites, stations and utilities are all up for grabs. Invest in houses and hotels, then watch the rent come pouring in! Make deals with other players and look out for bargains at auction. There are many ways to get what you want. For really speedy dealers, use the speed die for a quick and intense game of Monopoly. So get on Go and trade your way to success!<br/><br/>Includes <span>gameboard</span>, <span>8 tokens</span>, <span>28 Title Deed cards</span>, <span>16 Chance cards</span>, <span>16 Community Chest cards</span>, <span>money pack</span>,<span> 32 houses</span>, <span>12 hotels</span>, 2 dice and instructions<br/><br/>•Features a speed die for a faster, more intense game<br/>•Includes the new token that was voted No. 1: the cat<br/><br/>  
    
12.     <div>For 3 to 5 players.</div><br/><br/>Ages 8 and up.<br/><br/>Monopoly and all related characters are trademarks of Hasbro.  
    
13.     </section>

Example encoded as [Microdata](https://en.wikipedia.org/wiki/Microdata_(HTML)) embedded in HTML.

1. <section itemscope itemtype="https://schema.org/Game">  
    
2.     <section itemprop="offers" itemscope itemtype="https://schema.org/Offer">  
    
3.       <span>Approx. Retail:</span>  
    
4.       <span itemprop="priceCurrency">$</span><span itemprop="price">17.99</span>  
    
5.       <a href="/monopoly-2/en_US/shop/where-to-buy.cfm?brand_guid=DAD28866-1C43-11DD-BD0B-0800200C9A66&prodName=Monopoly%20Game" itemprop="availableAtOrFrom">Where To Buy</a>  
    
6.     </section>  
    
7.     <span itemprop="audience" itemscope itemtype="https://schema.org/PeopleAudience">  
    
8.       Ages: <span itemprop="suggestedMinAge">8</span> YEARS &amp; UP  
    
9.     </span>  
    
10.     <h4>Game Description:</h4>  
    
11.     <p itemprop="description">Own it all as a high-flying trader in the fast-paced world of real estate. Tour the city for the hottest properties: sites, stations and utilities are all up for grabs. Invest in houses and hotels, then watch the rent come pouring in! Make deals with other players and look out for bargains at auction. There are many ways to get what you want. For really speedy dealers, use the speed die for a quick and intense game of Monopoly. So get on Go and trade your way to success!<br/><br/>Includes <span itemprop="gameItem">gameboard</span>, <span itemprop="gameItem">8 tokens</span>, <span itemprop="gameItem">28 Title Deed cards</span>, <span itemprop="gameItem">16 Chance cards</span>, <span itemprop="gameItem">16 Community Chest cards</span>, <span itemprop="gameItem">money pack</span>,<span itemprop="gameItem"> 32 houses</span>, <span itemprop="gameItem">12 hotels</span>, 2 dice and instructions<br/><br/>•Features a speed die for a faster, more intense game<br/>•Includes the new token that was voted No. 1: the cat<br/><br/>  
    
12.     <div itemprop="numberOfPlayers" itemscope itemtype="https://schema.org/QuantitativeValue">For <span itemprop="minValue">3</span> to <span itemprop="maxValue">5</span> players.</div><br/><br/>Ages 8 and up.<br/><br/>Monopoly and all related characters are trademarks of <span itemprop="copyrightHolder">Hasbro</span>.  
    
13.     </section>

Example encoded as [RDFa](https://en.wikipedia.org/wiki/RDFa) embedded in HTML.

1. <section vocab="https://schema.org/" typeof="Game">  
    
2.     <section property="offers" typeof="Offer">  
    
3.       <span>Approx. Retail:</span>  
    
4.       <span property="priceCurrency">$</span><span property="price">17.99</span>  
    
5.       <a href="/monopoly-2/en_US/shop/where-to-buy.cfm?brand_guid=DAD28866-1C43-11DD-BD0B-0800200C9A66&prodName=Monopoly%20Game" property="availableAtOrFrom">Where To Buy</a>  
    
6.     </section>  
    
7.     <span property="audience" typeof="PeopleAudience">  
    
8.       Ages: <span property="suggestedMinAge">8</span> YEARS &amp; UP  
    
9.     </span>  
    
10.     <h4>Game Description:</h4>  
    
11.     <p property="description">Own it all as a high-flying trader in the fast-paced world of real estate. Tour the city for the hottest properties: sites, stations and utilities are all up for grabs. Invest in houses and hotels, then watch the rent come pouring in! Make deals with other players and look out for bargains at auction. There are many ways to get what you want. For really speedy dealers, use the speed die for a quick and intense game of Monopoly. So get on Go and trade your way to success!<br/><br/>Includes <span property="gameItem">gameboard</span>, <span property="gameItem">8 tokens</span>, <span property="gameItem">28 Title Deed cards</span>, <span property="gameItem">16 Chance cards</span>, <span property="gameItem">16 Community Chest cards</span>, <span property="gameItem">money pack</span>,<span property="gameItem"> 32 houses</span>, <span property="gameItem">12 hotels</span>, 2 dice and instructions<br/><br/>•Features a speed die for a faster, more intense game<br/>•Includes the new token that was voted No. 1: the cat<br/><br/>  
    
12.     <div property="numberOfPlayers" typeof="QuantitativeValue">For <span property="minValue">3</span> to <span property="maxValue">5</span> players.</div><br/><br/>Ages 8 and up.<br/><br/>Monopoly and all related characters are trademarks of <span property="copyrightHolder">Hasbro</span>.  
    
13.     </section>

Example encoded as [JSON-LD](https://en.wikipedia.org/wiki/JSON-LD) in a HTML script tag.

1. <script type="application/ld+json">  
    
2. {  
    
3.   "@context": "https://schema.org",  
    
4.   "@type": "Game",  
    
5.   "offers":{  
    
6.     "@type":"Offer",  
    
7.     "priceCurrency":"$",  
    
8.     "price":"17.99",  
    
9.     "availableAtOrFrom":"/monopoly-2/en_US/shop/where-to-buy.cfm?brand_guid=DAD28866-1C43-11DD-BD0B-0800200C9A66&prodName=Monopoly%20Game"  
    
10.   },  
    
11.   "audience":{  
    
12.     "@type":"PeopleAudience",  
    
13.     "suggestedMinAge":"8"  
    
14.   },  
    
15.   "description":"Own it all as a high-flying trader in the fast-paced world of real estate. Tour the city for the hottest properties: sites, stations and utilities are all up for grabs. Invest in houses and hotels, then watch the rent come pouring in! Make deals with other players and look out for bargains at auction. There are many ways to get what you want. For really speedy dealers, use the speed die for a quick and intense game of Monopoly. So get on Go and trade your way to success!",  
    
16.   "gameItem":["gameboard","8 tokens","Title Deed cards","16 Chance cards", "16 Community Chest cards","money pack","32 houses","12 hotels"],  
    
17.   "numberOfPlayers":{  
    
18.     "@type":"QuantitativeValue",  
    
19.     "minValue":"3",  
    
20.     "maxValue":"5"  
    
21.   },  
    
22.   "copyrightHolder":"Hasbro"  
    
23. }  
    
24. </script>

Structured representation of the JSON-LD example.

{ "@context": "https://schema.org", "@type": "Game", "offers":{ "@type":"Offer", "priceCurrency":"$", "price":"17.99", "availableAtOrFrom":"/monopoly-2/en_US/shop/where-to-buy.cfm?brand_guid=DAD28866-1C43-11DD-BD0B-0800200C9A66&prodName=Monopoly%20Game" }, "audience":{ "@type":"PeopleAudience", "suggestedMinAge":"8" }, "description":"Own it all as a high-flying trader in the fast-paced world of real estate. Tour the city for the hottest properties: sites, stations and utilities are all up for grabs. Invest in houses and hotels, then watch the rent come pouring in! Make deals with other players and look out for bargains at auction. There are many ways to get what you want. For really speedy dealers, use the speed die for a quick and intense game of Monopoly. So get on Go and trade your way to success!", "gameItem":["gameboard","8 tokens","Title Deed cards","16 Chance cards", "16 Community Chest cards","money pack","32 houses","12 hotels"], "numberOfPlayers":{ "@type":"QuantitativeValue", "minValue":"3", "maxValue":"5" }, "copyrightHolder":"Hasbro" }

V26.0  
2024-02-12

[Terms and conditions](/docs/terms.html)

 

|   |   |
|---|---|
|||