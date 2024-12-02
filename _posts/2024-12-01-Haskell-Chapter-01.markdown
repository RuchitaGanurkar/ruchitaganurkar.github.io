---
layout: post
title: "Data Types"
date:   2024-12-01 12:00:00 +0530
---

# 🚀 **Haskell Types Overview**

Welcome to the ultimate guide to Haskell types! 
This document covers **Sum Types** and all other major types in Haskell, with detailed explanations and practical examples. 
Let's dive in! 🚀


## 📖 **1. Sum Types**
Sum types represent values that can be one of many alternatives. 
They're perfect for modeling the data with multiple "cases."


- Example of a Sum Type
> data Shape = 
        Circle Float 
    |   Rectangle Float Float 
    |   Triangle Float Float Float


-  Example of a Product Type
> data Point = Point Int Int



-  Example of a Record Type
> data Employee = Employee { name :: String, age :: Int }


-  Example of a Newtype
> newtype UserId = UserId Int



-  Example of a Polymorphic Type
> data Box a = Box a



-  Example of an Enum Type
> data Color = 
        Red
    |   Green 
    |   Blue



-  Example of a Recursive Type
> data List a = 
        Empty 
    |   Cons a (List a)



-  Example of a Phantom Type
> data Phantom a = Phantom



-  Example of an Existential Type
> data Showable = forall a. Show a => MkShowable a


-  Example of a GADT \      
> data Expr a where \
  IntLit :: Int -> Expr Int \
  BoolLit :: Bool -> Expr Bool \
  Add :: Expr Int -> Expr Int -> Expr Int \
  If :: Expr Bool -> Expr a -> Expr a -> Expr a



-  Example of a Type Synonym
> type StringAlias = String



-  Example of a Tuple \
> pair = (1, "Hello")



-  Example of a List \
> numbers = [1, 2, 3, 4]



-  Example of Maybe Type
> data Maybe a = 
        Nothing
    |   Just a


-  Example of Either Type
> data Either a b = 
        Left a
    |   Right b


-  Example of Unit Type
> unit = ()

-  Example of a Function Type
> add :: Int -> Int -> Int \
> add x y = x + y



🔑 Conclusion

Haskell offers a wide variety of types to model > data with precision, flexibility, and safety. 
From simple Sum Types to powerful GADTs, you can choose the best tool for the job. 
Explore these types to write robust and expressive Haskell programs! 🛠️✨






