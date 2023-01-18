<div align="center">
	<h1><img alt="Stocks logo" src="https://github.com/octolibs/nyse-schedule/blob/main/timetable.png" height="300" /><br />
		Go New York Stock Exchange (NYSE) Schedule Library
	</h1>

[![Go Reference](https://pkg.go.dev/badge/octolibs/nyse-schedule.svg)](https://pkg.go.dev/github.com/octolibs/nyse-schedule) [![Go Version](https://img.shields.io/github/go-mod/go-version/octolibs/nyse-schedule)](https://go.dev/) [![GoReportCard](https://goreportcard.com/badge/github.com/octolibs/nyse-schedule)](https://goreportcard.com/report/github.com/octolibs/nyse-schedule) [![CodeFactor](https://www.codefactor.io/repository/github/octolibs/nyse-schedule/badge)](https://www.codefactor.io/repository/github/octolibs/nyse-schedule) [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/octolibs/nyse-schedule/.github/workflows/go.yml)](https://github.com/octolibs/nyse-schedule/blob/main/.github/workflows/go.yml) ![Size](https://img.shields.io/github/languages/code-size/octolibs/nyse-schedule) [![Last Commit](https://img.shields.io/github/last-commit/octolibs/nyse-schedule)](https://github.com/octolibs/nyse-schedule/commits/main) [![License](https://img.shields.io/github/license/octolibs/nyse-schedule)](https://github.com/octolibs/nyse-schedule/blob/main/LICENSE)

</div>
<hr/>

## 🌟 How it works

The library uses the current time to determine if the market is open, closed, or early closed. It also determines if the current day is a holiday.

## 📦 Installation and Usage

### Go

Make sure you have `Go` installed on your machine.

You can check by running the following command in the `console`

```plain
go version
```

If you don't have `Go` installed, you can download it from [here](https://go.dev/dl/).

### Add to your project

Run the following command in the `console`, in the `project directory`, to install the library with `go get`

```plain
go get github.com/octolibs/nyse-schedule
```

### Importing

Add the import to your `.go` file

```go
import "github.com/octolibs/nyse-schedule"
```

## 💰 Usage

### Check if the Market is Open at Current Time

```go
// Returns: bool
open := nyse_time.IsMarketOpen()
```

### Check if the Market will be Open based on a specific time and date

```go
// Parameters: time.Time
// Returns: bool
open := nyse_time.IsMarketOpenCustom(time.Time)
```

### Is Holiday?

```go
// Parameters: time.Time
// Returns: bool
isHoliday := nyse_time.IsHoliday(time.Time)
```

### Is Early Close?

```go
// Parameters: time.Time
// Returns: bool
isEarlyClose := nyse_time.IsEarlyClose(time.Time)
```

### Is Weekend?

```go
// Parameters: time.Time
// Returns: bool
isWeekend := nyse_time.IsWeekend(time.Time)
```

## 💻 Dependencies

- [`Go`](https://go.dev/)

## 🙇‍♂️ Issues and Contributing

If you find an issue with this library, please report an issue. If you'd
like, we welcome any contributions. Fork this library and submit a pull
request.

## ⚖️ License

This project is under the MIT License. See the [LICENSE](https://github.com/octolibs/nyse-schedule/blob/main/LICENSE) file for the full license text.

## 📜 Changes

Check out our [CHANGELOG](https://github.com/octolibs/nyse-schedule/blob/main/CHANGELOG.md)
