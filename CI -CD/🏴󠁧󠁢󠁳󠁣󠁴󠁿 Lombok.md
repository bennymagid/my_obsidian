#cicd
See License.java example below from `coverdash_common`
Can use `License.builder().id("id1").build();`
```
package com.coverdash.coverdash_common.api;  
  
import com.coverdash.coverdash_common.api.enums.IntegrationType;  
import com.fasterxml.jackson.annotation.JsonFormat;  
import com.fasterxml.jackson.annotation.JsonIgnore;  
import com.fasterxml.jackson.annotation.JsonIgnoreProperties;  
import lombok.*;  
import org.hibernate.annotations.CreationTimestamp;  
import org.hibernate.annotations.GenericGenerator;  
  
import javax.persistence.*;  
import java.io.Serializable;  
import java.time.LocalDateTime;  
import java.util.Arrays;  
import java.util.List;  
import java.util.Set;  
import java.util.stream.Collectors;  
  
@Table(name = "License")  
@Entity(name = "License")  
@JsonIgnoreProperties(ignoreUnknown = true)  
@NoArgsConstructor  
@AllArgsConstructor  
@Builder  
@Data  
public class License implements Serializable {  
    private static final long serialVersionUID = 1L;  
  
    @Id  
    @GeneratedValue(generator = "uuid")  
    @GenericGenerator(name = "uuid", strategy = "uuid2")  
    @Column(name = "id")  
    private String id;  
  
    @CreationTimestamp  
    @Column(name = "createdAt")  
    @JsonFormat(pattern="yyyy-MM-dd HH:mm:ss")  
    private LocalDateTime createdAt;  
  
    @Column(name = "name")  
    private String name;  
  
    @Column(name = "policyType")  
    private String policyType;  
  
    @Column(name = "companyType")  
    private String companyType;  
  
    @Column(name = "theme")  
    private String theme;  
  
    @Column(name = "allowedCarriers")  
    private String allowedCarriers;  
  
    @Column(name = "clientId")  
    private String clientId;  
  
    @Column(name = "logoUrl")  
    private String logoUrl;  
  
    @Column(name = "preferredCarrier")  
    private String preferredCarrier;  
  
    @Column(name = "disabledQuestions")  
    private String disabledQuestions;  
  
    @Column(name = "postPurchasePortalUrl")  
    private String postPurchasePortalUrl;  
  
    @Column(name = "partnerBio")  
    private String partnerBio;  
  
    @Column(name = "leadSellingEnabled")  
    private Boolean leadSellingEnabled;  
  
    @Column(name = "preEmptiveQuotingEnabled")  
    private Boolean preEmptiveQuotingEnabled;  
  
    @OneToMany(cascade = CascadeType.ALL, fetch = FetchType.LAZY)  
    @JoinColumn(name = "licenseName", referencedColumnName = "name")  
    private List<RecommendedPolicy> recommendedPolicies;  
  
    @ManyToOne  
    @JoinColumn(  
            name = "partnerPreferencesId",  
            referencedColumnName = "id",  
            foreignKey = @ForeignKey(  
                    name = "License_partnerPreferencesId_fkey"  
            )  
    )    private PartnerPreferences partnerPreferences;  
  
    @Column(name = "parentLicenseId")  
    private String parentLicenseId;  
  
    @Column(name = "integrationType")  
    private IntegrationType integrationType;  
  
    @Deprecated  
    public License(String id, String name, String policyType, String companyType, String allowedCarriers) {  
        this.id = id;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.allowedCarriers = allowedCarriers;  
    }  
    @Deprecated  
    public License(String id, String name, String policyType, String companyType, String theme, String allowedCarriers) {  
        this.id = id;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
    }  
    @Deprecated  
    public License(String id, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId) {  
        this.id = id;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
    }  
    @Deprecated  
    public License(String id, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String disabledQuestions) {  
        this.id = id;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.disabledQuestions = disabledQuestions;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String disabledQuestions) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.disabledQuestions = disabledQuestions;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String logoUrl, String disabledQuestions) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.logoUrl = logoUrl;  
        this.disabledQuestions = disabledQuestions;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String logoUrl, String preferredCarrier, String disabledQuestions) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.logoUrl = logoUrl;  
        this.preferredCarrier = preferredCarrier;  
        this.disabledQuestions = disabledQuestions;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String logoUrl, String preferredCarrier, String disabledQuestions, Boolean preEmptiveQuotingEnabled) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.logoUrl = logoUrl;  
        this.preferredCarrier = preferredCarrier;  
        this.disabledQuestions = disabledQuestions;  
        this.preEmptiveQuotingEnabled = preEmptiveQuotingEnabled;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String logoUrl, String preferredCarrier, String disabledQuestions, Boolean preEmptiveQuotingEnabled, List<RecommendedPolicy> recommendedPolicies) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.logoUrl = logoUrl;  
        this.preferredCarrier = preferredCarrier;  
        this.disabledQuestions = disabledQuestions;  
        this.preEmptiveQuotingEnabled = preEmptiveQuotingEnabled;  
        this.recommendedPolicies = recommendedPolicies;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String logoUrl, String preferredCarrier, String disabledQuestions, String postPurchasePortalUrl, Boolean preEmptiveQuotingEnabled, List<RecommendedPolicy> recommendedPolicies) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.logoUrl = logoUrl;  
        this.preferredCarrier = preferredCarrier;  
        this.disabledQuestions = disabledQuestions;  
        this.postPurchasePortalUrl = postPurchasePortalUrl;  
        this.preEmptiveQuotingEnabled = preEmptiveQuotingEnabled;  
        this.recommendedPolicies = recommendedPolicies;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String logoUrl, String preferredCarrier, String disabledQuestions, String postPurchasePortalUrl, Boolean leadSellingEnabled, Boolean preEmptiveQuotingEnabled, List<RecommendedPolicy> recommendedPolicies) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.logoUrl = logoUrl;  
        this.preferredCarrier = preferredCarrier;  
        this.disabledQuestions = disabledQuestions;  
        this.postPurchasePortalUrl = postPurchasePortalUrl;  
        this.leadSellingEnabled = leadSellingEnabled;  
        this.preEmptiveQuotingEnabled = preEmptiveQuotingEnabled;  
        this.recommendedPolicies = recommendedPolicies;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String logoUrl, String preferredCarrier, String disabledQuestions, String postPurchasePortalUrl, Boolean leadSellingEnabled, Boolean preEmptiveQuotingEnabled, List<RecommendedPolicy> recommendedPolicies, PartnerPreferences partnerPreferences) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.logoUrl = logoUrl;  
        this.preferredCarrier = preferredCarrier;  
        this.disabledQuestions = disabledQuestions;  
        this.postPurchasePortalUrl = postPurchasePortalUrl;  
        this.leadSellingEnabled = leadSellingEnabled;  
        this.preEmptiveQuotingEnabled = preEmptiveQuotingEnabled;  
        this.recommendedPolicies = recommendedPolicies;  
        this.partnerPreferences = partnerPreferences;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String logoUrl, String preferredCarrier, String disabledQuestions, String postPurchasePortalUrl, String partnerBio, Boolean leadSellingEnabled, Boolean preEmptiveQuotingEnabled, List<RecommendedPolicy> recommendedPolicies, PartnerPreferences partnerPreferences) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.logoUrl = logoUrl;  
        this.preferredCarrier = preferredCarrier;  
        this.disabledQuestions = disabledQuestions;  
        this.postPurchasePortalUrl = postPurchasePortalUrl;  
        this.partnerBio = partnerBio;  
        this.leadSellingEnabled = leadSellingEnabled;  
        this.preEmptiveQuotingEnabled = preEmptiveQuotingEnabled;  
        this.recommendedPolicies = recommendedPolicies;  
        this.partnerPreferences = partnerPreferences;  
    }  
    @Deprecated  
    public License(String id, LocalDateTime createdAt, String name, String policyType, String companyType, String theme, String allowedCarriers, String clientId, String logoUrl, String preferredCarrier, String disabledQuestions, String postPurchasePortalUrl, String partnerBio, Boolean leadSellingEnabled, Boolean preEmptiveQuotingEnabled, List<RecommendedPolicy> recommendedPolicies, PartnerPreferences partnerPreferences, String parentLicenseId) {  
        this.id = id;  
        this.createdAt = createdAt;  
        this.name = name;  
        this.policyType = policyType;  
        this.companyType = companyType;  
        this.theme = theme;  
        this.allowedCarriers = allowedCarriers;  
        this.clientId = clientId;  
        this.logoUrl = logoUrl;  
        this.preferredCarrier = preferredCarrier;  
        this.disabledQuestions = disabledQuestions;  
        this.postPurchasePortalUrl = postPurchasePortalUrl;  
        this.partnerBio = partnerBio;  
        this.leadSellingEnabled = leadSellingEnabled;  
        this.preEmptiveQuotingEnabled = preEmptiveQuotingEnabled;  
        this.recommendedPolicies = recommendedPolicies;  
        this.partnerPreferences = partnerPreferences;  
        this.parentLicenseId = parentLicenseId;  
    }  
    @JsonIgnore  
    public Set<String> getAllowedCarriersSet(){  
        return Arrays.stream(allowedCarriers.split(",")).collect(Collectors.toSet());  
    }  
    public String[] getDisabledQuestions() {  
        return disabledQuestions != null ? disabledQuestions.split(",") : new String[0];  
    }  
    public Boolean getPreEmptiveQuotingEnabled() {  
        return preEmptiveQuotingEnabled != null && preEmptiveQuotingEnabled;  
    }  
    public Boolean getLeadSellingEnabled() {  
        return leadSellingEnabled != null ? leadSellingEnabled : false;  
    }  
    @Override  
    public String toString() {  
        return "License{" +  
                "id='" + id + '\'' +  
                ", createdAt=" + createdAt +  
                ", name='" + name + '\'' +  
                ", policyType='" + policyType + '\'' +  
                ", companyType='" + companyType + '\'' +  
                ", theme='" + theme + '\'' +  
                ", allowedCarriers='" + allowedCarriers + '\'' +  
                ", clientId='" + clientId + '\'' +  
                ", logoUrl='" + logoUrl + '\'' +  
                ", preferredCarrier='" + preferredCarrier + '\'' +  
                ", disabledQuestions='" + disabledQuestions + '\'' +  
                ", postPurchasePortalUrl='" + postPurchasePortalUrl + '\'' +  
                ", partnerBio='" + partnerBio + '\'' +  
                ", leadSellingEnabled=" + leadSellingEnabled +  
                ", preEmptiveQuotingEnabled=" + preEmptiveQuotingEnabled +  
                ", recommendedPolicies=" + recommendedPolicies +  
                ", partnerPreferences=" + partnerPreferences +  
                ", parentLicenseId='" + parentLicenseId +  
                ", integrationType='" + integrationType +  
                '}';  
    }}
```