 ## GENERAL_LIABILITY ##
This GL Policy was bound (mistakenly BOP from the POV of CNA): **`43ace202-5445-4789-a751-937bc402fc57`**
here's one that was GL: `3b47f267-c2d2-453e-9214-7854c5a6b5c8`

All lines with filler data have been marked with a `//thisIsFiller`
Using this bind Request
```
{
    "SignonRq": {
        "ClientApp": {
            "Org": "TEST", //thisIsFiller
            "Name": "API" //thisIsFiller
        },
        "SignonPswd": {
            "CustId": {
                "CustLoginId": "TESTAPI"
            }
        }
    },
    "InsuranceSvcRq": [
        {
            "BOPPolicyAddRq": [
                {
                    "Producer": [
                        {
                            "ProducerInfo": {
                                "ContractNumber": {
                                    "value": "018297"
                                },
                                "com.cna_branchCode": [
                                    {
                                        "value": "010"
                                    }
                                ]
                            },
                            "GeneralPartyInfo": {
                                "NameInfo": [
                                    {
                                        "PersonName": {
                                            "Surname": {
                                                "value": "Smith" //thisIsFiller
                                            },
                                            "GivenName": {
                                                "value": "John" //thisIsFiller
                                            }
                                        }
                                    }
                                ]
                            }
                        }
                    ],
                    "CommlPolicy": {
                        "LOBCd": {
                            "value": "BOP" //thisIsFiller
                        },
                        "QuoteInfo": {
                            "CompanysQuoteNumber": {
                                "value": "11053870"
                            },
                            "com.cna_CompanysOptionNumber": {
                                "value": "0" //thisIsFiller
                            }
                        },
                        "PaymentOption": [
                            {
                                "PaymentPlanCd": {
                                    "value": "9E" //thisIsFiller
                                },
                                "DownPaymentPct": {
                                    "value": 25 //thisIsFiller
                                }
                            }
                        ],
                        "BillingMethodCd": {
                            "value": "CAB" //thisIsFiller
                        }
                    },
                    "BOPLineBusiness": {
                        "LOBCd": {
                            "value": "BOP" //thisIsFiller
                        }
                    }
                }
            ]
        }
    ]
}
```

And this quote request
```
{
    "OrgInfo": {
        "OrgId": {
            "value": "CNA"
        }
    },
    "InsuranceSvcRq": [
        {
            "BOPPolicyQuoteInqRq": [
                {
                    "ProductCd": {
                        "value": "CNAConnect"
                    },
                    "InsuredOrPrincipal": [
                        {
                            "InsuredOrPrincipalInfo": {
                                "BusinessInfo": {
                                    "NumEmployeesFullTime": {
                                        "value": 0 //thisIsFiller
                                    },
                                    "NumEmployeesPartTime": {
                                        "value": 0 //thisIsFiller
                                    },
                                    "SICCd": {
                                        "value": "73710_50" //thisIsFiller
                                    }
                                },
                                "BusinessTypeCd": {
                                    "value": "Other" //thisIsFiller
                                }
                            },
                            "GeneralPartyInfo": {
                                "NameInfo": [
                                    {
                                        "CommlName": {
                                            "CommercialName": {
                                                "value": "IS Biz"
                                            }
                                        },
                                        "LegalEntityCd": {
                                            "value": "LL"
                                        }
                                    }
                                ],
                                "Communications": {
                                    "PhoneInfo": [
                                        {
                                            "PhoneNumber": {
                                                "value": "554-378-9863"
                                            },
                                            "PhoneTypeCd": {
                                                "value": "Phone"
                                            }
                                        }
                                    ]
                                }
                            }
                        }
                    ],
                    "CommlSubLocation": [
                        {
                            "Construction": {
                                "BldgArea": {
                                    "NumUnits": {
                                        "value": 23000 //thisIsFiller
                                    }
                                },
                                "NumStories": {
                                    "value": 5 //thisIsFiller
                                },
                                "YearBuilt": {
                                    "value": 2010 //thisIsFiller
                                },
                                "ConstructionCd": [
                                    {
                                        "value": "JM" //thisIsFiller
                                    }
                                ]
                            },
                            "LocationRef": "L1"
                        }
                    ],
                    "CommlPolicy": {
                        "CommlPolicySupplement": {
                            "LengthTimeInBusiness": {
                                "NumUnits": {
                                    "value": 7 
                                }
                            },
                            "com.cna_CommlPolicySupplement": {
                                "BusinessInterruptionQuestion": {
                                    "YesNoCd": {
                                        "value": "NO" //thisIsFiller
                                    }
                                }
                            }
                        },
                        "NumLosses": {
                            "value": 0 //thisIsFiller
                        },
                        "ContractTerm": {
                            "EffectiveDt": {
                                "value": "2025-05-27"
                            }
                        }
                    },
                    "BOPLineBusiness": {
                        "com.cna_QuestionAnswer": [
                            {
                                "com.cna_QuestionCd": {
                                    "value": "UWSTMT" //thisIsFiller
                                },
                                "YesNoCd": {
                                    "value": "YES" //thisIsFiller
                                }
                            },
                            {
                                "com.cna_QuestionCd": {
                                    "value": "com.cna_TechnologyRestrictedActivities" //thisIsFiller
                                },
                                "YesNoCd": {
                                    "value": "NO" //thisIsFiller
                                }
                            }
                        ],
                        "PropertyInfo": {
                            "CommlPropertyInfo": [
                                {
                                    "CommlCoverage": [
                                        {
                                            "Deductible": [
                                                {
                                                    "FormatInteger": {
                                                        "value": 1000 //thisIsFiller
                                                    }
                                                }
                                            ],
                                            "CoverageCd": {
                                                "value": "BLDG"
                                            }
                                        },
                                        {
                                            "Limit": [
                                                {
                                                    "FormatInteger": {
                                                        "value": 1000 //thisIsFiller
                                                    }
                                                }
                                            ],
                                            "CoverageCd": {
                                                "value": "BPP"
                                            }
                                        }
                                    ],
                                    "ItemValueAmt": {
                                        "Amt": {
                                            "value": 1 //thisIsFiller
                                        }
                                    },
                                    "LocationRef": "L1"
                                }
                            ]
                        },
                        "LiabilityInfo": {
                            "GeneralLiabilityClassification": [
                                {
                                    "LocationRef": "L1"
                                }
                            ]
                        }
                    },
                    "Location": [
                        {
                            "id": "L1",
                            "Addr": {
                                "Addr1": {
                                    "value": "220 Millburn Ave"
                                },
                                "PostalCode": {
                                    "value": "07041"
                                },
                                "City": {
                                    "value": "Millburn"
                                },
                                "StateProvCd": {
                                    "value": "NJ"
                                },
                                "AddrTypeCd": [
                                    {
                                        "value": "MailingAddress"
                                    }
                                ]
                            }
                        }
                    ]
                }
            ],
            "WorkCompPolicyQuoteInq": [
                {
                    "RqUID": "19bab694-7da8-4e22-a"
                }
            ]
        }
    ],
    "SignonRq": {
        "ClientApp": {
            "Org": "TEST", //thisIsFiller
            "Name": "GreatAgentCompany" //thisIsFiller
        },
        "SignonPswd": {
            "CustId": {
                "CustLoginId": "TEST" //thisIsFiller
            }
        }
    }
}
```

But we should note that the following fields were prepopulated by CNA apparently
```
"ExtendedStatus": [
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlPolicy.ControllingStateProvCd"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlPolicy.CommlPolicySupplement['com.cna_LengthTimeIndustyManagement']"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlPolicy.ContractTerm.ExpirationDt"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlSubLocation[0].BldgProtection.DistanceToFireStation"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlSubLocation[0].BldgProtection.DistanceToHydrant"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlSubLocation[0].Construction.NumBasements.value"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlSubLocation[0].Construction['com.cna_UnfinishedBasementArea].NumUnits.value"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlSubLocation[0].Construction['com.cna_FinishedBasementArea].NumUnits.value"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlSubLocation[0].BldgImprovements.RoofingImprovementYear"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlSubLocation[0].BldgImprovements.WiringImprovementYear"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].CommlSubLocation[0].BldgOccupancy[0]['com.cna_OccupancyTypeCd']"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].BOPLineBusiness.PropertyInfo.CommlPropertyInfo[0].CommlCoverages[CoverageCd='WH']"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    },
    {
        "ExtendedStatusDesc": {
            "value": "CNA has defaulted this info in order to provide a quote, verify the value for your insured."
        },
        "MissingElementPath": [
            {
                "value": "$.InsuranceSvcRq[0].BOPPolicyQuoteInqRq[0].BOPLineBusiness.PropertyInfo.CommlPropertyInfo[0].CommlCoverages[CoverageCd='GLASS']"
            }
        ],
        "ExtendedStatusCd": {
            "value": "VerifyDataAbsence"
        }
    }
]
```