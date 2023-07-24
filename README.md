# StockExchange
stock data featch

    1. nse_main() -
    2. CSV Model -
        Convert Payload json data  data to CSV using Data frame 
        read CSV File => data = pd.read_csv(filename)
        Featch Csv Columns=> data.columns
        target = data.iloc[:, 5:]
        method- csv_data_model(filename,symbol,start_date,end_date)
        parameter -  filename, symbol, start_date, end_date

    3. Graph Model - 
        csv file data(CSV Model) represent as  graphical  format 
        Method - graph(data,symbol,start_date,end_date)
        parameter – data – CSV data  , symbol,start_date,end_date

        use - 
        symbol = 'BAJFINANCE
        series = 'EQ'
        start_date = ('12-05-2023')
        end_date = ('12-06-2023')
        data = pd.read_csv(filename)
        graph(data,symbol,start_date,end_date)

    4. Equity Pre Data-
        Equity pre histary featch 
        Method - equity_predata(symbol, series, start_date, end_date)
        parameter – Symbol, series, Start Date, End Date 
        Use - 
        symbol = 'BAJFINANCE
        series = 'EQ'
        start_date = ('12-05-2023')
        end_date = ('12-06-2023')
        equity_predata(symbol, series, start_date, end_date)

        Output - 
            • Create CSV File  of start date to end date  data 
                _id
                CH_SYMBOL
                Outcome
                CH_SERIES
                CH_MARKET_TYPE
                CH_TRADE_HIGH_PRICE
                CH_TRADE_LOW_PRICE
                CH_OPENING_PRICE
                CH_CLOSING_PRICE
                CH_LAST_TRADED_PRICE
                CH_LAST_TRADED_PRICE
                CH_PREVIOUS_CLS_PRICE
                CH_TOT_TRADED_QTY
                CH_TOT_TRADED_VAL
                CH_52WEEK_HIGH_PRICE
                CH_52WEEK_LOW_PRICE
                CH_TOTAL_TRADES
                CH_ISIN
                CH_TIMESTAMP
                TIMESTAMP
                createdAt
                updatedAt
                __v
                VWAP
                mTIMESTAMP

            • Plot graph in linear scal  using Graph method 
