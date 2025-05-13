```mermaid
graph TD

%% ------- 0. Keskuskäsitteet (Central Concepts) --------
    Economies("Taloudet (Economies)")
    Markets("Markkinat (Markets)")
    Globalization("Globalisaatio (Globalization)")
    InterestRate("Korko (Interest rate)")

%% ------- 1. Yleinen Talous (General Economy) --------
    subgraph YleinenTalous["Yleinen Talous (General Economy)"]
        direction LR
        GEG["Maailmantalouden kasvu (Global economic growth)"]
        Recession["Lama/Taantuma (Recession)"]
        EcoDownturn["Taloussuhdanteen lasku (Economic downturn)"]
        EcoIndicator["Talousindikaattori (Economic indicator)"]
        GDP["BKT (Gross Domestic Product)"]
        PerCapGDP["BKT per asukas (Per capita GDP)"]
        GNP_GNI["BKTL/BKT (Gross National Product/Income)"]
        Inflation["Inflaatio (Inflation)"]
        CPI["KHI (Consumer Price Index)"]
        Deflation["Deflaatio (Deflation)"]
        Outlook["Näkymät (Outlook)"]
        Forecast["Ennuste (Forecast)"]
        LeadInd["Ennakoivat indikaattorit (Leading indicators)"]
        Economist["Ekonomisti (Economist)"]
        EcoTheory["Talousteoria (Economic theory)"]
        Econometrics["Ekonometria (Econometrics)"]

        Economies --> GEG
        GEG --> Recession
        GEG --> EcoDownturn
        EcoDownturn -.-> Recession
        Economies --> EcoIndicator
        EcoIndicator --> GDP
        GDP --> PerCapGDP
        EcoIndicator --> GNP_GNI
        EcoIndicator --> Inflation
        Inflation --> CPI
        EcoIndicator --> Deflation
        Economies --> Outlook
        Outlook --> Forecast
        Forecast --> LeadInd
        Economist --> EcoTheory
        Economist --> Econometrics
    end

%% ------- 2. Markkinat ja Sijoittaminen (Markets and Investing) --------
    subgraph MarkkinatSijoittaminen["Markkinat ja Sijoittaminen (Markets and Investing)"]
        direction LR
        FinMarket["Rahoitusmarkkinat (Financial market)"]
        StockMarket["Osakemarkkinat (Stock market)"]
        StockExchanges["Pörssit (Stock exchanges)"]
        Nasdaq["Nasdaq (Nasdaq)"]
        Stocks["Osakkeet (Stocks)"]
        Equity["Oma Pääoma (Equity)"]
        Securities["Arvopaperit (Securities)"]
        MarketCap["Markkina-arvo (Market capitalization)"]
        IPO["Listautumisanti (Initial Public Offering)"]
        CapitalMarkets["Pääomamarkkinat (Capital markets)"]
        BondMarket["Joukkovelkakirjamarkkinat (Bond market)"]
        Bonds["Joukkovelkakirjat (Bonds)"]
        USTreasuryYields["USA:n valtionlainojen tuotot (U.S. Treasury yields)"]
        Commodity["Hyödyke (Commodity)"]
        OilPrices["Öljyn hinta (Oil prices)"]
        EnergySector["Energia-ala (Energy sector)"]
        Trading["Kaupankäynti (Trading)"]
        Broker["Välittäjä (Broker)"]
        Investors["Sijoittajat (Investors)"]
        Portfolio["Salkku (Portfolio)"]
        RiskMgmt["Riskienhallinta (Risk management)"]
        MarketSenti["Markkinatunnelma/-liikkeet (Market Sentiment/Movements)"]
        Rally["Nousuralli (Rally)"]
        BullMarket["Nousumarkkina (Bull market)"]
        BearMarket["Laskumarkkina (Bear market)"]
        MarketCorr["Markkinakorjaus (Market correction)"]
        Tumbling["Romahtaminen (Tumbling)"]
        Rebounded["Elpyminen (Rebounded)"]
        Losses["Tappiot (Losses)"]
        Profit["Voitto (Profit)"]
        StockIndex["Osakeindeksi (Stock market index)"]
        SP500["S&P 500 (S&P 500)"]
        HSI["Hang Seng -indeksi (Hang Seng Index)"]
        Stoxx600["Stoxx 600 -indeksi (Stoxx 600 index)"]
        IndexFund["Indeksirahasto (Index fund)"]
        Benchmark["Vertailuindeksi (Benchmark)"]

        Markets --> FinMarket
        Markets --> Commodity
        Commodity --> OilPrices
        OilPrices --> EnergySector
        FinMarket --> StockMarket
        FinMarket --> CapitalMarkets
        FinMarket --> BondMarket
        StockMarket --> StockExchanges
        StockExchanges --> Nasdaq
        StockMarket --> Securities
        Securities --> Stocks
        Stocks -.-> Equity["Oma pääoma (Equity)"]
        Securities --> Bonds
        StockMarket --> MarketCap
        Stocks --> MarketCap
        StockMarket --> IPO
        CapitalMarkets --> Securities
        CapitalMarkets --> BondMarket
        CapitalMarkets --> StockMarket
        BondMarket --> Bonds
        Bonds --> USTreasuryYields
        USTreasuryYields --> InterestRate
        
        Markets --> Trading
        Trading --> Broker
        Trading --> Investors
        Investors --> Portfolio
        Investors --> RiskMgmt
        
        Markets --> MarketSenti
        MarketSenti --> Rally
        Rally -.-> BullMarket
        MarketSenti --> BullMarket
        MarketSenti --> BearMarket
        MarketSenti --> MarketCorr
        MarketSenti --> Tumbling
        MarketSenti --> Rebounded
        Trading --> Losses
        Trading --> Profit
        Losses --- Profit
        
        StockMarket --> StockIndex
        StockIndex --> SP500
        StockIndex --> HSI
        StockIndex --> Stoxx600
        StockIndex --> IndexFund
        StockIndex -.-> Benchmark
        SP500 -.-> Benchmark
        HSI -.-> Benchmark
        Stoxx600 -.-> Benchmark
    end

%% ------- 3. Kansainvälinen Kauppa (International Trade) --------
    subgraph KansKauppa["Kansainvälinen Kauppa (International Trade)"]
        direction LR
        TradePolicy["Kauppapolitiikka (Trade policy)"]
        Tariffs["Tullit (Tariffs)"]
        ImportDuty["Tuontitulli (Import duty)"]
        Quota["Kiintiö (Quota)"]
        Subsidy["Tukiainen (Subsidy)"]
        TradeBarriers["Kaupan esteet (Trade barriers)"]
        NTBs["Ei-tullimuotoiset esteet (Non-tariff barriers)"]
        Protectionism["Protektionismi (Protectionism)"]
        FTA["Vapaakauppasopimus (Free trade agreement)"]
        Dumping["Polkumyynti (Dumping)"]
        FairTrade["Reilu kauppa (Fair trade)"]
        TradeWar["Kauppasota (Trade war)"]
        TradeNeg["Kauppaneuvottelut (Trade negotiations)"]
        Concession["Myönnytys (Concession)"]
        JointStmt["Yhteinen julkilausuma (Joint statement)"]
        BilateralAgr["Kahdenvälinen sopimus (Bilateral agreement)"]
        MultilateralAgr["Monenkeskinen sopimus (Multilateral agreement)"]
        Imports["Tuonti (Imports)"]
        Exports["Vienti (Exports)"]
        BalanceTrade["Kauppatase (Balance of trade)"]
        TradeSurplus["Ylijäämäinen kauppatase (Trade surplus)"]
        TradeDeficit["Alijäämäinen kauppatase (Trade deficit)"]
        Goods["Tavarat (Goods)"]
        Services["Palvelut (Services)"]
        TradeRel["Kauppasuhde (Trade relationship)"]

        Globalization --> KansKauppa
        KansKauppa --> TradePolicy
        TradePolicy --> Tariffs
        Tariffs --- ImportDuty
        TradePolicy --> Quota
        TradePolicy --> Subsidy
        TradePolicy --> TradeBarriers
        TradeBarriers --> Tariffs
        TradeBarriers --> Quota
        TradeBarriers --> NTBs
        TradePolicy --> Protectionism
        TradePolicy --> FTA
        TradePolicy --> Dumping
        TradePolicy --> FairTrade
        KansKauppa --> TradeWar
        TradeWar -.-> Tariffs
        TradeWar -.-> TradePolicy
        KansKauppa --> TradeNeg
        TradeNeg --> Concession
        TradeNeg --> JointStmt
        TradeNeg --> BilateralAgr
        TradeNeg --> MultilateralAgr
        FTA -.-> BilateralAgr
        FTA -.-> MultilateralAgr
        
        KansKauppa --> Imports
        KansKauppa --> Exports
        Imports --> Goods
        Imports --> Services
        Exports --> Goods
        Exports --> Services
        Imports -.-> BalanceTrade
        Exports -.-> BalanceTrade
        BalanceTrade --> TradeSurplus
        BalanceTrade --> TradeDeficit
        
        KansKauppa --> TradeRel
        Economies --> TradeRel
    end

%% ------- 4. Valuutat ja Valuuttamarkkinat (Currencies and Foreign Exchange) --------
    subgraph ValuutatFX["Valuutat ja Valuuttamarkkinat (Currencies and Foreign Exchange)"]
        direction LR
        CurrenciesVal["Valuutat (Currencies)"]
        USDollar["USA:n dollari (U.S. dollar)"]
        ExchangeRate["Valuuttakurssi (Exchange rate)"]
        FXResearch["Valuuttatutkimus (Foreign exchange research)"]
        CurrencyRisk["Valuuttariski (Currency risk)"]
        Hedging["Suojautuminen (Hedging)"]

        FinMarket --> CurrenciesVal
        CurrenciesVal --> USDollar
        CurrenciesVal --> ExchangeRate
        ExchangeRate --> FXResearch
        FXResearch --> CurrencyRisk
        FXResearch --> Hedging
        RiskMgmt -.-> Hedging
        Trading -.-> Hedging
    end

%% ------- 5. Talouspolitiikka (Economic Policy) --------
    subgraph Talouspolitiikka["Talouspolitiikka (Economic Policy)"]
        direction LR
        MonetaryPolicy["Rahapolitiikka (Monetary policy)"]
        CentralBank["Keskuspankki (Central bank)"]
        Fed["Federal Reserve (Fed)"]
        MoneySupply["Rahan tarjonta (Money supply)"]
        FiscalPolicy["Finanssipolitiikka (Fiscal policy)"]
        Stimulus["Elvytyspaketti (Stimulus package)"]

        Economies --> Talouspolitiikka
        Talouspolitiikka --> MonetaryPolicy
        MonetaryPolicy --> CentralBank
        CentralBank --> Fed
        MonetaryPolicy --> MoneySupply
        MonetaryPolicy --> InterestRate
        
        Talouspolitiikka --> FiscalPolicy
        FiscalPolicy --> Stimulus
        FiscalPolicy --> Subsidy
        FiscalPolicy --> Tariffs
    end

%% ------- 6. Kansainväliset Organisaatiot ja Ryhmät (International Organizations and Groups) --------
    subgraph KansToimijat["Kansainväliset Organisaatiot ja Ryhmät (International Actors)"]
        direction LR
        WTO["Maailman kauppajärjestö (WTO)"]
        IMF["Kansainvälinen valuuttarahasto (IMF)"]
        G7["G7-ryhmä (Group of 7)"]

        KansToimijat --> WTO
        WTO --> TradePolicy
        WTO --> TradeNeg
        Globalization -.-> WTO
        KansToimijat --> IMF
        IMF --> Economies
        IMF --> MonetaryPolicy
        IMF --> Outlook
        IMF --> CurrenciesVal
        Globalization -.-> IMF
        KansToimijat --> G7
        G7 --> GEG
        G7 --> TradePolicy
        G7 --> Economies
        Globalization -.-> G7
    end

%% ------- Yhteydet pääkäsitteiden välillä --------
    Economies --> Markets
    Markets --> Globalization
    Globalization --> Economies

    Investors --> Economies
    TradePolicy --> Economies
    GEG --> Markets
    BondMarket --> InterestRate
```
